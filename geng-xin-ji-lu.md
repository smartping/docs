#更新记录

- **2017.09.26 SMARTPING v0.4.1 RELEASE**

```
- 修订拓扑图自身节点显示红线BUG
```



- **2017.09.15 SMARTPING v0.4.0 RELEASE**

```
- 增加日志支持[基于seelog]
- 修订使用系统Ping命令的取值方法，支持Win/Linux/Mac
- 增加用户选择使用系统Ping或GoPing[基于go-fastping]的选项（推荐使用SysPing，若存在兼容性问题时选用-GoPing）
- Windows下增加后台运行服务支持[基于nssm],并可使用双击control.cmd运行SmartPing
- Linux下增加pack指令，可以快速将SmartPing进行编译并打包
- WebDashbord中AgentList更名为SmartPing NetWork
- 修订部分数据类型
```

- **2017.09.16 SMARTPING v0.3.1 RELEASE**

```
- 修订计算算法，每3s发送一个ping包,每分钟发送20个，计算其最高,最低,平均延迟、丢包率。
- API接口header变更为json
- 修复拓扑节点自动刷新失效问题
```


- **2017.09.16 SMARTPING v0.3.0 RELEASE**

```
- 全新的Dashbord设计，支持报警数据存储，配置WEB管理
- 更新数据结构，进行数据拆表
- 开放API接口，Dashbord数据全部采用API接口方式通过Ajax获取
- 修订了一大堆的BUG
- 项目官网上线smartping.org，文档上线docs.smartping.org
```

- **2017.09.12 SMARTPING v0.2.5 RELEASE**

```
 -
```


- **2017.07.17 SMARTPING v0.2.4 RELEASE**

```
 -
```