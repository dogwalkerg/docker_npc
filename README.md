# docker_npc
nps⁠的客户端npc

一款轻量级、功能强大的内网穿透代理服务器。支持tcp、udp流量转发，支持内网http代理、内网socks5代理，同时支持snappy压缩、站点保护、加密传输、多路复用、header修改等。支持web图形化管理，集成多用户模式。

使用方式

docker pull ffdfgdfg/npc

下载conf文件夹⁠并解压，或前往项目主页⁠自行下载**(升级请忽略)**

继续阅读文档⁠按照不同的启动方式启动**(升级请忽略)**

无配置文件：docker run -d --name npc --net=host ffdfgdfg/npc -server=<ip:port> -vkey=<web界面中显示的密钥> <以及一些其他参数>

配置文件：docker run -d --name npc --net=host -v <本机conf目录>:/conf ffdfgdfg/npc -config=/conf/npc.conf

参数附在后面即可请确保为conf文件夹下的npc.conf

查看日志docker logs npc
