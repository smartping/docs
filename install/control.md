# 脚本参数

smartping采用脚本调用方式运行，Linux使用 ./control , Windows使用 control.cmd

## Linux

 **./control**

```text
build|run|start|stop|restart|status

build   : 源码编译，最终构建成至 bin
run     : 直接启动smartping
start   : 以nohup(deamon)形式启动smartping
stop    : 关闭smartping
restart : 执行 stop & start
status  : 查看smartping的运行状态
version : 查看当前smartping版本
pack    : 执行Build并进行二进制包制作
```

## Windows

 **control.cmd** 

```text
build|run|install|start|stop|restart|version

build   : 源码编译，最终构建成至 bin
run     : 直接启动smartping
install : 使用nssm将smartping安装为服务
start   : 启动smartping服务
stop    : 关闭smartping服务
restart : 执行 stop & start
version : 显示当前smartping版本
```

