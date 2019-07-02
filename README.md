# 介绍

SmartPing是一个综合性网络质量\(PING\)检测工具，支持正/反向PING绘图、互PING拓扑绘图与报警、全国PING延迟地图与在线检测工具等功能。

## 功能

* 正向PING，反向Ping绘图
* 互PING间机器的状态拓扑，自定义延迟、丢包阈值报警（声音报警与邮件报警），报警时MTR检测
* 全国PING延迟地图（各省份可分电信、联通、移动三条线路）
* 检测工具，支持使用SmartPing各节点进行网络相关检测

## 设计思路

本系统的定位为轻量级工具，即使组多点成互Ping网络可以遵守无中心化原则，所有的数据均存储自身节点中，每个节点提供出方向的数据，从任意节点查询数据均会通过Ajax请求关联节点的API接口获取并组装全部数据。

* [数据去中心化](https://docs.smartping.org/arch/decentralized.html)

* [存储数据结构](https://docs.smartping.org/arch/data.html)
* [集中配置管理\(云模式\)](https://docs.smartping.org/arch/cloud.html)

## 功能截图

正/反向Ping![](/assets/index.jpg)

Ping拓扑及报警![](/assets/topology.jpg)![](/assets/alert.jpg)延迟地图![](/assets/map.jpg)

检测工具![](/assets/tools.jpg)

系统配置![](/assets/config.jpg)

