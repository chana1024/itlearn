# ngnix 编译 
/configure --with-http_stub_status_module --with-http_ssl_module 
make 
make install 
* 默认安装位置为/usr/local/nginx
* 编译完后，整个默认nginx目录即是二进制运行包，拷走即可运行
* ldd nginx可以查看nginx需要哪些动态链接库
# docker 安装
** cmd ENTRYPOINT 介绍,cmd ENTRYPOINT均只能由一个，多个是只有最后一个生效，所以子镜像会覆盖父镜像
** 要运行多个服务，建议cmd或ENTRYPOINT,指定sh脚本运行。服务命令写在脚本里
** 容器里的主进程要显示运行,主进程退出，容器也会退出
** multi stage多阶段构建
** 网路问题，容器如何localhost访问主机
** 体积优化问题，是否要用alpine
** 每个命令都会导致多一层镜像，CMD，RUN，ADD等。docker history可以查看层数
** -e参数会通过设置环境变量传递参数

