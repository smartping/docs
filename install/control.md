#脚本参数
smartping采用脚本调用方式运行，Linux使用 ./control , Windows使用 control.cmd 

##Linux
** ./control**

```
build|run|start|stop|restart|status

build   : 源码编译，最终构建成至 bin
run     : 直接启动smartping
start   : 以nohup(deamon)形式启动smartping
stop    : 关闭smartping
restart : 执行 stop & start
status  : 查看smartping的运行状态
```

##Windows
** control.cmd **

```
build|run|start|stop|restart|status

build   : 源码编译，最终构建成至 bin
run     : 直接启动smartping
start   : 使用[nssm](http://www.nssm.cc/)将smartping安装成服务并启动
stop    : 关闭smartping并卸载服务
restart : 执行 stop & start
status  : 查看smartping的运行状态
```

