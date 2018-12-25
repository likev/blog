---
title: Sina App Engine(SAE)中的Mysql服务限制说明
tags:
  - mysql
  - sae
  - 限制
id: 1019
categories:
  - mysql
  - 互联网
date: 2011-11-23 14:02:18
---

Mysql服务概要 

    SAE平台为每个App支持几乎所有MySQL的特性。目前支持MyISAM引擎，暂不支持InnoDB。需要注意的是SAE的数据库需要显式开启或者禁用。您还可以通过phpmyadmin来创建数据库和数据表。SAE的PHP环境提供了标准的MYSQL,MYSQLI和PDO模块(基于MySQLnd)，您可以直接使用这三个模块来操作您的数据库， 您可以使用预定义常量来连接数据库，我们不排除未来可能调整数据库端口，使用预定义常量能够避免这样的问题。当然SAE也提供了SaeMysql类，我们也推荐您使用这个类来操作MySQL资源。

服务限制
<table cellspacing="1" cellpadding="1" style="width: 600px">
			<tbody>
				<tr>
					<td>限制</td>
					<td>相关错误信息</td>
					<td>数值</td>
				</tr>
				<tr>
					<td>单表的最大行数</td>
					<td>Table too many rows</td>
					<td>10 000 000 行</td>
				</tr>
				<tr>
					<td>库的最大表数量</td>
					<td>Too many tables</td>
					<td>512个</td>
				</tr>
				<tr>
					<td>不支持的存储引擎类型</td>
					<td>Not support table type</td>
					<td>memory temporary</td>
				</tr>
				<tr>
					<td>最大外排序的行数</td>
					<td>Filesort on too many rows</td>
					<td>65536 行</td>
				</tr>
				<tr>
					<td>最大无索引的操作行数</td>
					<td>无</td>
					<td>100 000 行</td>
				</tr>
				<tr>
					<td>查询的最大操作行数</td>
					<td>Select on too many rows</td>
					<td>1 000 000 行</td>
				</tr>
				<tr>
					<td>更新的最大操作行数</td>
					<td>Update on too many rows</td>
					<td>1 000 000 行</td>
				</tr>
				<tr>
					<td>删除的最大操作行数</td>
					<td>Delete on too many rows</td>
					<td>1 000 000 行</td>
				</tr>
				<tr>
					<td>创建索引时允许的表的最大行数</td>
					<td>Create index on big table</td>
					<td>500 000 行</td>
				</tr>
				<tr>
					<td>修改表结构时允许的表的最大行数</td>
					<td>Alter table on big table</td>
					<td>500 000 行</td>
				</tr>
				<tr>
					<td>SQL并发执行时间和(读库)</td>
					<td>Operations take too much time cost</td>
					<td>500 000 毫秒</td>
				</tr>
				<tr>
					<td>SQL并发执行时间和(写库)</td>
					<td>Operations take too much time cost</td>
					<td>200 000 毫秒</td>
				</tr>
				<tr>
					<td>警报阈值百分比</td>
					<td>无</td>
					<td>80%</td>
				</tr>
				<tr>
					<td>表主键及聚簇索引奖励系数</td>
					<td>无</td>
					<td>1024 倍</td>
				</tr>
			</tbody>
		</table>

 MySQL慢查询配额

SQL执行时间超过1秒，即为慢查询，其分钟配额为
条目数 	10
累计执行时间 	30秒
扫描行 	1,000,000

 分钟配额
    运行在SAE上的应用(App)将会消耗平台资源，为保证各App不互相影响，我们引入了分钟配额的概念，即：在每分钟内每个应用的各个服务所消耗的 资源的速度。比如，当平台中的某个应用的MySQLl服务一分钟内累计请求数达到20万，或者流出宽带超过600M，或者累计CPU执行时间超过400s，我们将会立即禁掉该应用的MySQL服务，禁用五分钟后，恢复会自动恢复，避免影响到SAE平台的稳定性。服务因为超过“分钟配额”而被禁用时，会在“服务状态”看到该服务被禁用的原因。

注意：表中红色配额值是自2011-11-3号，即SAE两周年起开始执行的新配额值，旧配额值将不再采用。
<table style="width: 578px; height: 316px" class="quota">
	<tbody>
		<tr>
			<td>服务</td>
			<td>请求数</td>
			<td>cpu时间</td>
			<td>流入流量</td>
			<td>流出流量</td>
		</tr>
		<tr>
			<td>HTTP</td>
			<td>200,000=&gt;<font color="#FF0000">500,000</font></td>
			<td>300s=&gt;<font color="#FF0000">600s</font></td>
			<td>300MB=&gt;<font color="#FF0000">1500MB</font></td>
			<td>300MB=&gt;<font color="#FF0000">1500MB</font></td>
		</tr>
		<tr>
			<td>HTTPS</td>
			<td>50,000=&gt;<font color="#FF0000">1,000,000</font></td>
			<td>50s=&gt;<font color="#FF0000">100s</font></td>
			<td>10MB=&gt;<font color="#FF0000">100MB</font></td>
			<td>10MB=&gt;<font color="#FF0000">100MB</font></td>
		</tr>
		<tr>
			<td>[MySQL](/?m=devcenter&amp;catId=192)</td>
			<td>200,000</td>
			<td>400s=&gt;<font color="#FF0000">600s</font></td>
			<td>300MB=&gt;<font color="#FF0000">600MB</font></td>
			<td>600MB=&gt;<font color="#FF0000">1200MB</font></td>
		</tr>
		<tr>
			<td>[Memcache](/?m=devcenter&amp;catId=201)</td>
			<td>300,000</td>
			<td>NA</td>
			<td>150MB=&gt;<font color="#FF0000">300MB</font></td>
			<td>150MB=&gt;<font color="#FF0000">300MB</font></td>
		</tr>
		<tr>
			<td>[Fetchurl](/?m=devcenter&amp;catId=197)</td>
			<td>50,000=&gt;<font color="#FF0000">100,000</font></td>
			<td>NA</td>
			<td>100MB=&gt;<font color="#FF0000">200MB</font></td>
			<td>100MB=&gt;<font color="#FF0000">200MB</font></td>
		</tr>
		<tr>
			<td>[Image](/?m=devcenter&amp;catId=198)</td>
			<td>5,000</td>
			<td>300s</td>
			<td>150MB</td>
			<td>150MB</td>
		</tr>
		<tr>
			<td>[Storage](/?m=devcenter&amp;catId=204)</td>
			<td>5,000</td>
			<td>NA</td>
			<td>50MB=&gt;<font color="#FF0000">80MB</font></td>
			<td>400MB</td>
		</tr>
		<tr>
			<td>[Mail](/?m=devcenter&amp;catId=200)</td>
			<td>50=&gt;<font color="#FF0000">500</font></td>
			<td>NA</td>
			<td>20MB</td>
			<td>20MB</td>
		</tr>
		<tr>
			<td>Cron/offset</td>
			<td>50</td>
			<td>50s</td>
			<td>1MB</td>
			<td>1MB</td>
		</tr>
		<tr>
			<td>Cron/nooffset</td>
			<td>200</td>
			<td>30s=&gt;<font color="#FF0000">60s</font></td>
			<td>5MB</td>
			<td>5MB</td>
		</tr>
		<tr>
			<td>[TaskQueue](/?m=devcenter&amp;catId=205)</td>
			<td>20,000=&gt;<font color="#FF0000">40,000</font></td>
			<td>60s=&gt;<font color="#FF0000">100s</font></td>
			<td>10MB=&gt;<font color="#FF0000">20MB</font></td>
			<td>10MB=&gt;<font color="#FF0000">20MB</font></td>
		</tr>
		<tr>
			<td>VerifyCode</td>
			<td>100</td>
			<td>4s</td>
			<td>2MB</td>
			<td>2MB</td>
		</tr>
		<tr>
			<td>[KVDB](/?m=devcenter&amp;catId=199)</td>
			<td>150,000=&gt;<font color="#FF0000">300,000</font></td>
			<td>NA</td>
			<td>150MB=&gt;<font color="#FF0000">300MB</font></td>
			<td>150MB=&gt;<font color="#FF0000">300MB</font></td>
		</tr>
	</tbody>
</table>

容量配额

    容量配额是针对MySQL\Storage\MemCache设置的，是指用户能够使用的磁盘或内存的最大限制(见下表)，其中Memcache的最大容量配额是用户自己在初始化Memcache时设置的，可设置的范围是1M~256M。
服务 	配额
MySQL 	5G
Storage 	10G*
KVDB 	100G
*每个App允许建立5个Storage domain 每个domain为2G