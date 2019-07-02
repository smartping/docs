# 数据结构

SmartPing采用Sqlite进行数据存储，且数据结构非常简单，项目中的database-base.db为一个空sqlite数据库，程序根据场景建立响应的数据存储表。

打开SmartPing的Sqlite数据库后可以看到，SmartPing共两种类型数据表

* pinglog-{IP}
* alertlog-{date}

## pinglog-{IP}

pinglog数据表根据用户所设置的检测机器生成，数据表logtime设置为唯一主键，存储日-小时-分\(例如:\[16 18:20\]16号18点20分\)数据，PING检测数据通过Replace Into形式写入保证循环存储1个月的数据,保证单表最大数据量为1440\*31=44640条，当用户去除响应节点检测时自动删除。

```text
CREATE TABLE [pinglog-{IP}] (
    logtime   VARCHAR (8),
    maxdelay  VARCHAR (3),
    mindelay  VARCHAR (3),
    avgdelay  VARCHAR (3),
    sendpk    VARCHAR (2),
    revcpk    VARCHAR (2),
    losspk    VARCHAR (3),
    lastcheck VARCHAR (16),
    PRIMARY KEY (
        logtime
    )
);
CREATE INDEX "lc" ON [pinglog-{IP}] (
        lastcheck
);
```

## alertlog-{date}

alertlog-{date}数据表根据用户设置的保留报警日志时常进行按日分表并定期清理

```text
CREATE TABLE [alertlog-20170916] (
    logtime   VARCHAR (8),
    fromname  VARCHAR (15),
    toname    VARCHAR (15),
    tracert   TEXT 
);
```

