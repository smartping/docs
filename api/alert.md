# alert

本节点将返回有效时间区域内的报警信息，默认参数为空时显示当日数据。注意：报警每分钟进行检测

## 接口方法

GET

## 接口地址

/api/alert.json

## 接口入参

| **参数** | **格式** | **示例** |
| :--- | :--- | :--- |
| date | alertlog-yyymmdd | alertlog-20170916 |

## 接口数据

```text
[
    [
        "alertlog-20170915",                    #报警日期列表
        "alertlog-20170916"
    ],
    [
        {
            "Logtime": "2017-09-16 15:22",      #报警时间
            "Fromname": "DESKTOP-EM9L0D5",      #来源名称
            "Toname": "114DNS",                 #目标名称
            "Tracert": "..."                    #Traceroute信息
        },
        {
            "Logtime": "2017-09-16 15:22",
            "Fromname": "DESKTOP-EM9L0D5",
            "Toname": "NOPING",
            "Tracert": "..."
        }
    ]
]
```

