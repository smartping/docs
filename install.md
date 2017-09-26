# 下载安装

## 二进制安装

### 选择相应OS的二进制包（最新版本v0.4.1）

* Linux： [Github](https://github.com/gy-games/smartping/releases/download/v0.4.1/smartping-v0.4.1.tar.gz) [百度云](https://pan.baidu.com/s/1o83c1w2)
* Windows：[Github](https://github.com/gy-games/smartping/releases/download/v0.4.1/smartping-v0.4.1.zip) [百度云](https://pan.baidu.com/s/1slodrKL)

All Release：[Github](https://github.com/gy-games/smartping/releases) [百度云](https://pan.baidu.com/s/1dFnflq5)

### 解压并运行程序

* 解压压缩包。
* 使用命令\(Windows使用CMD\) cd 进入到刚刚创建的目录。
* 执行命令 
* * **Linux:** ./control start 
* * **Windows:** 双击 control.cmd

** SmartPing默认WEB服务端口为8899，管理界面默认密码为:smartping,若需要修改请修改conf/config.json或conf/config-base.json **

## 源码安装

### 基本依赖

* Go 语言：版本 &gt;= 1.6

### 安装GO语言

如果您的系统已经安装要求版本的 Go 语言，可以跳过。

安装参考：[https://studygolang.com/dl](https://studygolang.com/dl)

### 源码编译

克隆或直接下载ZIP的源码包

* git clone [https://github.com/gy-games/smartping.git](https://github.com/gy-games/smartping.git)
* cd smartping
* * **Linux:** ./control build
* * **Windows:** control.cmd build

### 运行程序

* * **Linux:** ./control start 
* * **Windows:** control.cmd start


** SmartPing默认WEB服务端口为8899，管理界面默认密码为:smartping,若需要修改请修改conf/config.json或conf/config-base.json **

