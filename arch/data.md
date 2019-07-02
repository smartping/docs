# 数据结构

SmartPing采用Sqlite进行数据存储，且数据结构非常简单，如果需要二次开发且对数据库操作比较熟悉，可以直接在此取数据

打开SmartPing的Sqlite数据库后可以看到，SmartPing总共三张表

* pinglog
* alertlog
* mappinglog

## pinglog

pinglog数据表存储正向Ping数据

```text
CREATE TABLE pinglog (
    logtime  VARCHAR (16),
    target   VARCHAR (15),
    maxdelay FLOAT,
    mindelay FLOAT,
    avgdelay FLOAT,
    sendpk   INT,
    revcpk   INT,
    losspk   INT
);

```

## alertlog

alertlog存储报警信息

```text
CREATE TABLE alertlog (
    logtime    VARCHAR (16),
    targetip   VARCHAR (16),
    targetname VARCHAR (15),
    tracert    TEXT
);

```

## mappinglog

mappinglog存储全国延迟检测信息

```text
CREATE TABLE mappinglog (
    logtime DATETIME,
    mapjson TEXT
);


```



