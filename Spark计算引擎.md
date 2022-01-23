# Spark计算引擎

标签（空格分隔）： 大数据 Hadoop spark

## Spark介绍
Spark是 一个通用的分布式计算框架。

## Spark组件

- Spark core

- Spark SQL

- Spark streaming

- Mlib

- Graphx

- Cluster Manager

---
## Spark环境搭建

- 运行环境
    java - 7以上版本

- 下载地址

- spark Shell
    pyspark 支持Python 的API
    
- spark 集群运行
    启动master：./sbin/start-master.sh
    启动worker：./bin/spark-class
    提交作业： ./bin/spark-submit

    

---
## Spark 模型 RDD

- Diver program
    通过sparkcontext访问spark

- RDDs (Resilient Distributed dataset)
    并行分布在整个集群中
    RDDs是spark分发和计算数据的抽象类

- RDDs包含函数
    map()
    filter()
    flatMap() 数据扁平化
- RDDs 常用Action
    collect()
    count()
    countByValue()
    take()
    top()
    takeOrdered()
    takeSimple()
    reduce()
    fold()
    aggregate()
    foreach()
- RDDs的特性
    1. 血统关系图
    2. 延迟计算（scala的语言特性）
    3. 持久化 persist()
        级别|空间占用|CPU消耗
        MEMORY_ONLY
        MEMORY_ONLY_SER
        DISK_ONLY
        MEMORY_AND_DISK
        MEMORY_AND_DISK_SER
- RDDs 对于key-value数据的处理
    reduceByKey()
    groupByKey()
    combineByKey()
    keys
    values
    sortByKey()
    mapValues()
    flatMapValues()
