# config

本接口将返回该节点的配置信息

## 接口方法

GET

## 接口地址

/api/config.json

## 接口入参

无

## 接口数据

```text
{
	"Ver": "0.8.0",
	"Port": 8899,
	"Name": "本机",
	"Addr": "127.0.0.1",
	"Mode": {
		"Endpoint": "",
		"LastSuccTime": "",
		"Status": "true",
		"Type": "local"
	},
	"Base": {
		"Archive": 10,
		"Refresh": 1,
		"Timeout": 5
	},
	"Topology": {
		"Tline": "1",
		"Tsound": "/alert.mp3",
		"Tsymbolsize": "70"
	},
	"Alert": {
		"EmailHost": "",
		"RevcEmailList": "",
		"SendEmailAccount": "",
		"SendEmailPassword": ""
	},
	"Network": {
		"1.2.3.4": {
			"Name": "OtherSP",
			"Addr": "1.2.3.4",
			"Smartping": true,
			"Ping": [
				"114.114.114.114",
				"127.0.0.1",
				"8.8.4.4"
			],
			"Topology": [
				{
					"Addr": "127.0.0.1",
					"Name": "本机",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "30",
					"Thdoccnum": "3"
				},
				{
					"Addr": "114.114.114.114",
					"Name": "114DNS",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "30",
					"Thdoccnum": "3"
				},
				{
					"Addr": "8.8.4.4",
					"Name": "GoogleDNS",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "30",
					"Thdoccnum": "3"
				},
				{
					"Addr": "1.2.3.4",
					"Name": "OtherSP",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "30",
					"Thdoccnum": "3"
				}
			]
		},
		"114.114.114.114": {
			"Name": "114DNS",
			"Addr": "114.114.114.114",
			"Smartping": false,
			"Ping": [],
			"Topology": []
		},
		"123.125.114.144": {
			"Name": "百度",
			"Addr": "123.125.114.144",
			"Smartping": false,
			"Ping": [],
			"Topology": []
		},
		"127.0.0.1": {
			"Name": "本机",
			"Addr": "127.0.0.1",
			"Smartping": true,
			"Ping": [
				"1.2.3.4",
				"114.114.114.114",
				"123.125.114.144",
				"127.0.0.1",
				"69.171.229.28",
				"8.8.4.4"
			],
			"Topology": [
				{
					"Addr": "1.2.3.4",
					"Name": "OtherSP",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "30",
					"Thdoccnum": "3"
				},
				{
					"Addr": "114.114.114.114",
					"Name": "114DNS",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "30",
					"Thdoccnum": "3"
				},
				{
					"Addr": "8.8.4.4",
					"Name": "GoogleDNS",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "10",
					"Thdoccnum": "3"
				},
				{
					"Addr": "69.171.229.28",
					"Name": "Facebook",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "30",
					"Thdoccnum": "3"
				},
				{
					"Addr": "123.125.114.144",
					"Name": "百度",
					"Thdavgdelay": "200",
					"Thdchecksec": "900",
					"Thdloss": "30",
					"Thdoccnum": "3"
				}
			]
		},
		"69.171.229.28": {
			"Name": "Facebook",
			"Addr": "69.171.229.28",
			"Smartping": false,
			"Ping": [],
			"Topology": []
		},
		"8.8.4.4": {
			"Name": "GoogleDNS",
			"Addr": "8.8.4.4",
			"Smartping": false,
			"Ping": [],
			"Topology": []
		}
	},
	"Chinamap": {
		"上海": {
			"cmcc": [
				"117.184.42.114"
			],
			"ctcc": [
				"180.163.15.160"
			],
			"cucc": [
				"223.167.104.117"
			]
		},
		"北京": {
			"cmcc": [
				"111.13.217.125"
			],
			"ctcc": [
				"120.92.180.135"
			],
			"cucc": [
				"111.207.189.5"
			]
		},
		"广东": {
			"cmcc": [
				"120.236.14.140"
			],
			"ctcc": [
				"218.17.216.171"
			],
			"cucc": [
				"58.252.2.194"
			]
		},
		"浙江": {
			"cmcc": [
				"183.246.69.139"
			],
			"ctcc": [
				"115.236.169.86"
			],
			"cucc": [
				"60.12.214.156"
			]
		}
	},
	"Toollimit": 0,
	"Authiplist": "",
	"Password": ""
}
```



