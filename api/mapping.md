# Mapping

本节点将返回全国延迟Ping数据，不加参数默认显示前一分钟的数据

## 接口方法

GET

## 接口地址

/api/mapping.json

## 接口入参

| **参数** | **格式** | **示例** |
| :--- | :--- | :--- |
| d | yyyy-mm-dd hh:mm | 2017-09-16 10:20 |

## 接口数据

```text
{
    "text": "本机",
    "subtext": "2019-07-02 16:02",
    "avgdelay": {
        "cmcc": [{                       //中国移动
            "value": 5.34,
            "name": "北京"
        }, {
            "value": 28.99,
            "name": "上海"
        }],
        "ctcc": [{                       //中国电信
            "value": 27.33,
            "name": "上海"
        }, {
            "value": 29,
            "name": "北京"
        }],
        "cucc": [{                      //中国联通
            "value": 3.33,
            "name": "北京"
        }, {
            "value": 28.99,
            "name": "上海"
        }]
    }
}
```



