#节点配置信息

## 接口数据
```
{
	"Ver": "0.3.0",                             #当前Smartping版本                
	"Port": 8890,                               #Smartping服务端口号
	"Name": "DESKTOP-EM9L0D5",                  #本机名称
	"Ip": "127.0.0.1",                          #本机IP
	"Db": "D:/smartping/db/database.db",        #Sqlite数据库路径
	"Password": "",                             #密码（此处将显示为空）
	"Alerthistory": 7,                          #报警数据存储周期（天）
	"Alertcycle": 1,                            #拓扑页面-刷新时间（分钟）
	"Alertsound": "/alert.mp3",                 #拓扑页面-报警声音
	"Thdchecksec": 900,                         #报警规则-监测时间范围（秒）
	"Thdoccnum": 3,                             #报警规则-在监控时间范围内出现的异常点数（个）
	"Thdavgdelay": 200,                         #报警规则-平均延迟（毫秒）
	"Thdloss": 30,                              #报警规则-丢包率（百分比）
	"Tline": "1",                               #拓扑页面-互PING点连接线粗细
	"Tsymbolsize": "70",                        #拓扑页面-互PING点图大小
	"Topotimeout": "5",                         #Ajax请求超时时间
	"Targets": [                             #目标机器列表
		{
		 	"Name": "本机",          #目标机器名称
			"Addr": "127.0.0.1",     #目标机器IP
			"Type": "CS",            #模式（CS:互PING,C:正向PING）  
			"Thdchecksec": 900,      #特殊报警规则-监测时间范围（秒）
			"Thdoccnum": 3,          #特殊报警规则-在监控时间范围内出现的异常点数（个）
			"Thdavgdelay": 200,      #特殊报警规则-平均延迟（毫秒）
			"Thdloss": 30            #特殊报警规则-丢包率（百分比）
		},
		{
			"Name": "NOPING",        #同上
			"Addr": "93.46.8.89",
			"Type": "C",
			"Thdchecksec": 900,
			"Thdoccnum": 3,
			"Thdavgdelay": 200,
			"Thdloss": 30
		},
		{
			"Name": "百度",
			"Addr": "220.181.57.217",
			"Type": "CS",
			"Thdchecksec": 900,
			"Thdoccnum": 3,
			"Thdavgdelay": 200,
			"Thdloss": 30
		},
		{
			"Name": "114DNS",
			"Addr": "114.114.114.114",
			"Type": "CS",
			"Thdchecksec": 30,
			"Thdoccnum": 3,
			"Thdavgdelay": 200,
			"Thdloss": 50
		}
	]
}
```