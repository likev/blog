---
title: 迅雷离线下载Javascript代码分析
id: 888
categories:
  - 未分类
date: 2011-10-02 17:06:32
tags:
---

<pre lang='javascript'>
function download_check(obj,arg){
    if(typeof(g_isfree)!='undefined' && g_isfree){//判断免费用户
        if(obj!=bt_task_down && obj!=thunder_download && obj!=batch_down_bt && obj!=rm_saveas && obj!=rm_saveas_bt){
            alert('免费用户不支持批量下载，请单个下载！');
            return false;
        }
        var bid = -1;
        if(obj==thunder_download){
            if(typeof(arg[1])=='undefined'){
                var taskid = arg[0];
            }
            else{//BT子任务，获取
                var taskid = $("#bttaskid"+arg[0].toString()).val();
                bid = arg[0];
            }
        }
        else if(obj == batch_down_bt){
            var taskid = $('#view_bt_taskid').val();
        }
        else if(obj == rm_saveas){
            var taskid = arg[0];
        }
        else if(obj == rm_saveas_bt){
            var bid = arg[0];
            var taskid = $("#bttaskid"+arg[0].toString()).val();
        }
        else{
            var taskid = arg[1];
        }
        var t = 0;
        var api = $('#free_down').pop({
            onHide:function(){
                try{
                    clearInterval(t);
                }
                catch(e){}
            }
        });
        $('#free_topicbox_2').hide().find('div').removeClass('bg_why');
        $('#free_conlist_2').hide();
        $('#free_topicbox_1').show();
        $('#free_conlist_1').show();
        $('#free_down_xz').show();
        $('#free_down_hy').hide();
        var hasclick = false;

        var that = $('#free_down_todown').html('普通下载').removeClass('btn_noit')
        .unbind('click')
        .bind('click',function(){
            if(hasclick) return;
            hasclick = true;
            var i=30;
            $.getScript(INTERFACE_URL + "/get_wait_time?callback=download_check_respo&taskid="+taskid+'&t='+new Date());
            window.download_check_respo = function(res){
                hasclick = false;
                if(res && res.result==0){
                    i=res.wait_time;
                    that.unbind('click');
                }
                else{
                    alert('出现异常，请刷新页面重试');
                    return false;
                }
                $('#free_topicbox_1,#free_conlist_1').hide();
                $('#free_topicbox_2,#free_conlist_2').show();
                $('#free_topicbox_2').find('div').addClass('bg_why');
                that.html('还剩'+i.toString()+'秒').addClass('btn_noit');
                t = setInterval(function(){
                    i--;
                    if(i&lt;=0){
                        try{
                            clearInterval(t);
                        }
                        catch(e){}
                        that.html('获取地址中...');
                        //function d(){
                            if(obj==bt_task_down){//下载BT任务
                            $.getJSON(INTERFACE_URL + '/get_wait_time?callback=?&t='+new Date(),{key:res.key,taskid:taskid,t:new Date()},function(process){
                                    if(process.result!=0){
                                        alert('出现异常，请刷新页面重试');
                                        return;
                                    }
                                    start_get_free_download_url();
                                });
                            }
                            else if(obj==batch_down_bt || obj==rm_saveas_bt){//bt_list
                            $.getJSON(INTERFACE_URL + "/free_get_url?callback=?&t="+new Date(),{key:res.key,list:taskid,bt_list:taskid,uid:getCookie('userid'),t:new Date()},function(process){
                                    if(process.result!=0){
                                        alert('出现异常，请刷新页面重试');
                                        return;
                                    }
                                    var o = process.list;
                                    $.each(o,function(i,v){
                                        $('input[name=btdownurl'+v.tid.toString()+']').val(v.lixian_url);
                                    });
                                    start_get_free_download_url();
                                });
                            }
                            else{
                            $.getJSON(INTERFACE_URL + "/free_get_url?callback=?&t="+new Date(),{key:res.key,list:taskid,nm_list:taskid,uid:getCookie('userid'),t:new Date()},function(process){
                                    if(process.result!=0){
                                        alert('出现异常，请刷新页面重试');
                                        return;
                                    }
                                    var o = process.list[0];
                                    if(bid==-1){
                                        $('#dl_url'+arg[0]).val(o.lixian_url);
                                    }
                                    else{//BT子任务
                                        $('#btdownurl'+bid.toString()).val(o.lixian_url);
                                        $('#bt_list'+bid.toString()).val(o.lixian_url);
                                    }
                                    start_get_free_download_url();
                                });
                            }
                        //}
                        //d();
                        function hasError(){
                        }
                        function start_get_free_download_url(){
                            that.html('开始下载').removeClass('btn_noit');
                            that.bind('click',function(){
                                api.hide();
                                todo();
                                return false;
                            });
                        }
                    }
                    else{
                        that.html('还剩'+i.toString()+'秒');
                    }
                },1*1000);
            }
            return false;
        });
        return false;
    }
    else{
        todo();
    }
    function todo(){
        var _a = [];
        for(var i=0;i<arg.length;i++){
            _a.push(arg[i]);
        }
        _a.push('download');
        obj.apply(this,_a);
    }
}
</pre>