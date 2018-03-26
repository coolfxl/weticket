# weticket
微信购票小程序+后台管理系统


引入项目到eclipse中，部署在tomcat中正常启动的日志文件

信息: Starting ProtocolHandler ["http-bio-8095"]

[INFO][2018-03-26 15:37:38] com.hqc.util.RedisUtil.clear(RedisUtil.java:109) Clear Key 

[INFO][2018-03-26 15:37:38] com.hqc.task.RedisTask.autoTask(RedisTask.java:37) 清空所有Redis缓存成功 

访问路径

#不带项目名
http://localhost:8095/hqc_mp/octopus/sys/index.html

#带项目名 
http://localhost:8095/octopus/sys/index.html

后台登录界面
用户名/密码：admin/admin

redis下载地址

https://download.csdn.net/download/dkjhl/10309147

启动redis

cd /usr/local/redis

./redis-server redis.conf

如果防火墙没有开放redis默认端口6379则关闭防火墙

service iptables stop

下面是后台部分截图和小城序部分截图

后台

![登录界面](https://github.com/coolfxl/weticket/blob/master/pictures/01.png)
![首页](https://github.com/coolfxl/weticket/blob/master/pictures/02.png)
![门片添加](https://github.com/coolfxl/weticket/blob/master/pictures/03.jpg)

小程序

![小程序首页](https://github.com/coolfxl/weticket/blob/master/pictures/04.jpg)
![小程序购票](https://github.com/coolfxl/weticket/blob/master/pictures/05.jpg)
