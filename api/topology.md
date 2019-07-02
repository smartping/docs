# topology

本节点将返回经过报警规则过滤后的目标节点状态,SmartPing Dashbord使用此数据来绘制拓扑

## 接口方法

GET

## 接口地址

/api/topology.json

## 接口入参

无

## 接口数据

```text
{
	"1.2.3.4": "false",
	"114.114.114.114": "true",
	"123.125.114.144": "true",
	"69.171.229.28": "false",
	"8.8.4.4": "false"
}
```

目标节点IP-&gt;状态\(treu,false\)

