# Tools

本节点将返回目标Ping结果数据，默认Ping5个数据包

## 接口方法

GET

## 接口地址

/api/tools.json

## 接口入参

| **参数** | **格式** | **示例** |
| :--- | :--- | :--- |
| t | ip or domain | 127.0.0.1 / smartping.org |

## 接口数据

```text
{
    "status": "true",
    "error": "",
    "ip": "127.0.0.1",
    "ping": {
        "SendPk": 5,
        "RevcPk": 5,
        "LossPk": 0,
        "MinDelay": 0,
        "AvgDelay": 0.59982,
        "MaxDelay": 0.9997
    }
}
```



