# API文档

SmartPing所有的数据均可以通过各点的程序通过HTTP方式获取（SmartPing Dashbord数据的展示同样调用以上接口获取），SmartPing的API接口均以打开Access-Control-Allow-Origin:\*支持跨域。

| **名称** | **METHOD** | **URI** | **介绍** |
| :--- | :--- | :--- | :--- |
| [当前节点配置信息](config.md) | GET | /api/config.json | 获取当前节点的配置信息 |
| [PING目标机器数据](ping.md) | GET | /api/ping.json | 获取当前节点对外的PING数据 |
| [PING目标机器状态](topology.md) | GET | /api/topology.json | 获取当前节点PING外部的状态数据（用于拓扑） |
| [PING目标机器报警数据](alert.md) | GET | /api/alert.json | 获取当前的报警数据 |

