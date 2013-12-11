###一、简介

Atlas是由 Qihoo 360,  Web平台部基础架构团队开发维护的一个基于MySQL协议的数据中间层项目。它在MySQL官方推出的MySQL-Proxy 0.8.2版本的基础上，修改了大量bug，添加了很多功能特性。目前该项目在360公司内部得到了广泛应用，很多MySQL业务已经接入了Atlas平台，每天承载的读写请求数达几十亿条。
    
主要功能：

(1).读写分离

(2).从库负载均衡

(3).IP过滤

(4).SQL语句黑白名单

(5).自动分表

(6).支持客户端以长连接的方式连接Atlas。

###二、Atlas相对于官方MySQL-Proxy的优势

(1).将主流程中所有Lua代码改为纯C实现，Lua仅用在管理接口。

(2).重写网络模型、线程模型。

(3).实现了真正意义的连接池。

(4).优化了锁机制，性能提高数十倍。

###三、Atlas详细说明


[1.Atlas的安装](http://github.com/Qihoo360/Atlas/wiki/Atlas的安装)
[2.Atlas的运行及常见问题](http://github.com/Qihoo360/Atlas/wiki/Atlas的运行及常见问题)
[3.Atlas的分表功能简介](http://github.com/Qihoo360/Atlas/wiki/Atlas的分表功能简介)


###附名字来源：

Atlas，希腊神话中双肩撑天的巨人，普罗米修斯的兄弟，最高大强壮的神之一，因反抗宙斯失败而被罚顶天。我们期望这个系统能够脚踏后端DB，为前端应用撑起一片天。

