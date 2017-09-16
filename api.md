# API文档

SmartPing所有的数据均可以通过各点的程序通过HTTP方式获取（SmartPing Dashbord数据的展示同样调用以上接口获取）

| **名称** | **METHOD** | **URI** | **介绍** |
| :--- | :--- | :--- | :--- |
| [当前节点配置信息](/api/config.md) | GET | /api/config.json | 获取当前节点的配置信息 |
| [PING目标机器数据](/api/ping.md) | GET | /api/ping.json | 获取当前节点对外的PING数据 |
| [PING目标机器状态](/api/topology.md) | GET | /api/topology.json | 获取当前节点PING外部的状态数据（用于拓扑） |
| [PING目标机器报警数据](/api/alert.md) | GET | /api/alert.json | 获取当前节点PING外部的状态数据（用于拓扑） |
| [修改当前节点配置信息](/api/saveconfig.md) | GET | /api/saveconfig.json | 修改当前节点的配置信息 |
