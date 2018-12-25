---
title: Google Maps 显示地面天气实况
tags:
  - maps
  - mysql
  - php
  - 天气
id: 960
categories:
  - mysql
  - php
date: 2011-11-07 00:32:07
---

## 一、用到的技术

1. Google Maps API
2. jQuery & jQuery UI &jqPlot
3. canvas 绘制风速及UI
4. mysql 站点信息表 & 站点-时间-观测数据 表 &其他信息表(站点和数据最近更新时间、最新数据时间)
5. php返回json形式站点信息并在客户端持久存储
6. Ajax轮询请求获取最新数据
7. GeoLocation获取用户地理位置并定位
8. 鼠标悬停站点时显示基本信息，点击detail时Ajax获取本站点最详尽信息
9. Javascript解析数据代码为天气信息，计算湿度和本站气压等
10. 统计某一段时间数据(单站数据或多站对比)
11. C++ 自动监测处理(去掉站点经纬度高度等信息)地面图文件并post数据 & 网页手动上传文件更新(提供基本上传和拖动上传方式)

<!-- more -->

> 地面填图文件示例：[11110620.000](http://grow-wordpress.stor.sinaapp.com/uploads/2011/11/11110620.000.txt)

## 二、代码实现

1. 创建站点数据表

    ```sql
    CREATE TABLE IF NOT EXISTS station(
    id INT UNSIGNED NOT NULL UNIQUE PRIMARY KEY ,
    lon DOUBLE NOT NULL ,
    lat DOUBLE NOT NULL ,
    height DOUBLE NOT NULL ,
    LEVEL TINYINT UNSIGNED NOT NULL ,
    name VARCHAR( 50 )
    );
    ```

2. 创建地面观测数据表

    ```sql
    CREATE TABLE IF NOT EXISTS surface(
    recordId int(10) unsigned NOT NULL AUTO_INCREMENT,
     stationId int(10) unsigned NOT NULL,
     recordTime datetime NOT NULL,
     totalCloudAmount smallint(5) unsigned NOT NULL,
     windDirection smallint(5) unsigned NOT NULL,
     windSpeed smallint(5) unsigned NOT NULL,
     seaLevelPressure smallint(5) unsigned NOT NULL,
     press3hour smallint(6) NOT NULL,
     pastWeather1 smallint(5) unsigned NOT NULL,
     pastWeather2 smallint(5) unsigned NOT NULL,
     hour6precipitation double NOT NULL,
     lowCloudAmount smallint(5) unsigned NOT NULL,
     lowCloudShape smallint(5) unsigned NOT NULL,
     lowCloudHight smallint(5) unsigned NOT NULL,
     dewpoint double NOT NULL,
     visibility double unsigned NOT NULL,
     presentWeather smallint(5) unsigned NOT NULL,
     temperature double NOT NULL,
     middleCloudShape smallint(5) unsigned NOT NULL,
     highCloudShape smallint(5) unsigned NOT NULL,
     transformT24 smallint(6) NOT NULL,
     transformPress24 smallint(6) NOT NULL,
     PRIMARY KEY (recordId),
     UNIQUE KEY stationId (stationId,recordTime)
    ) ENGINE=MyISAM DEFAULT CHARSET=utf8
    ```

    每个月数据约100万行，可每个月建立一张表
    ```sql
    CREATE TABLE IF NOT EXISTS `surface201111` LIKE surface;
    ```

3. 插入数据到station表

    ```php
    function update_stations($content){
    	preg_match_all('/^(\d{5})\s+(-?\d+\.\d+)\s+(-?\d+\.\d+)\s+(-?\d+)\s+(\d+)/m',$content,$matchs,PREG_SET_ORDER);

    	//print_r($matchs);

    	$sql = 'INSERT IGNORE INTO station (id, lon, lat, height, level) VALUES ';

    	for($i = 0; $i < count($matchs); $i++){
    		$sql .= '( ';

    		for($j = 1; $j < 5; $j++){
    			$sql .= $matchs[$i][$j].",";
    		}
    		$sql .= $matchs[$i][5] .' )';
    		if($i < count($matchs) - 1)
    		{
    			$sql .= ',';
    		}
    	}
    	//echo $sql;

    	$mydb = new DB(SAE_MYSQL_HOST_M);
    	return $mydb -> doSql($sql);
    }
    ```
4. 插入数据到surface表

    ```php
    function getSurfacePatten(){
    	$patten = '/^(\d{5})(?:\s+-?\d+\.\d+){2}(?:\s+-?\d+\s+\d+)';

    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(-?\d+)';
    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(\d+)';

    	$patten .= '\s+(\d*\.\d+|\d+)';

    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(\d+)';

    	$patten .= '\s+(-?\d*\.\d+|\d+)';
    	$patten .= '\s+(\d*\.\d+|\d+)';
    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(-?\d*\.\d+|\d+)';

    	$patten .= '\s+(\d+)';
    	$patten .= '\s+(\d+)';

    	$patten .= '\s+\d+';
    	$patten .= '\s+\d+';

    	$patten .= '\s+(-?\d+)';
    	$patten .= '\s+(-?\d+)';

    	$patten .= '/m';

    	return $patten;
    }

    function update_surface($content){

    	preg_match('/(\d+)\s+(0?\d+)\s+(0?\d+)\s+(0?\d+)\s+(\d+)\s*$/m',$content,$matchs);

    	$year = $matchs[1] > '50' ? '19'.$matchs[1] : '20'.$matchs[1];
    	$timestr = $year.$matchs[2].$matchs[3].$matchs[4].'0000';

    	$patten = getSurfacePatten();

    	preg_match_all($patten,$content,$matchs,PREG_SET_ORDER);

    	//print_r($matchs);

    	$sql = 'INSERT IGNORE INTO surface (';
    	$sql .= 'recordTime,stationID,';
    	$sql .= 'totalCloudAmount,windDirection,windSpeed,seaLevelPressure,press3hour,pastWeather1,pastWeather2,';
    	$sql .= 'hour6precipitation,lowCloudAmount,lowCloudShape,lowCloudHight,';
    	$sql .= 'dewpoint,visibility,presentWeather,temperature,';
    	$sql .= 'middleCloudShape,highCloudShape,';
    	$sql .= 'transformT24,transformPress24';
    	$sql .= ' ) VALUES ';

    	$mydb = new DB(SAE_MYSQL_HOST_M);

    	for($i = 0; $i < count($matchs); $i++){
    		$isexist = $mydb -> rows_of_select('select * from surface where stationId = '.$matchs[$i][1].' and recordTime = '.$timestr);

    		if($isexist > 0) continue;

    		$sql .= '( ';
    		$sql .= $timestr.",";

    		for($j = 1; $j < 20; $j++){
    			$str = $matchs[$i][$j].",";
    			$sql .= $str[0] === '.' ? '0'.$str : $str;
    		}
    		$sql .= $matchs[$i][20] .' )';
    		if($i < count($matchs) - 1)
    		{
    			$sql .= ', ';
    		}
    	}

    	return $mydb -> doSql($sql);
    }
    ```

5. 更新站点信息(站点名称)
    ```sql
    update station set name = '顺义' where id=54398;
    update station set name = '海淀' where id=54399;
    update station set name = '延庆' where id=54406;
    update station set name = '佛爷顶' where id=54410;
    update station set name = '汤河口' where id=54412;
    update station set name = '密云' where id=54416;
    update station set name = '怀柔' where id=54419;
    update station set name = '密云上甸子' where id=54421;
    update station set name = '平谷' where id=54424;
    update station set name = '通州' where id=54431;
    update station set name = '朝阳' where id=54433;
    update station set name = '昌平' where id=54499;
    update station set name = '斋堂' where id=54501;
    ```

6. 根据用户请求返回数据：

    ```sql
    SELECT id, lon, lat,
    LEVEL
    FROM station
    WHERE LEVEL <=2
    ORDER BY sqrt( lon * lon + lat * lat )
    LIMIT 30
    ```

7. 检查是否有重复数据
    ```sql
    SELECT recordTime, stationId, count( recordTime ) AS num
    FROM `surface`
    WHERE recordTime =20111111230000
    GROUP BY stationId
    LIMIT 500
    ```

8. 添加唯一性约束条件
    ```sql
    delete FROM `surface`
    WHERE stationId =99999;

    alter table surface
    add unique (stationId,recordTime);
    ```
