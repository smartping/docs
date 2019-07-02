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
    "114DNS": "true",
    "NOPING": "false",
    "本机": "true",
    "百度": "true"
}
```

目标节点名称-&gt;状态\(treu,false\)

