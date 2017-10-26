# 第2节 mongodb 介绍及安装

https://www.mongodb.com/

关系型数据库(sql) 和非关系型数据库(nosql)


mongodb
 是一款 nosql 数据库   

 
面向文档(collection)的数据库

存储数据格式 bson

1. mongodb的安装

2. 创建数据目录
 data

3. 启动服务端

D:\MongoDB\Server\3.2\bin\mongod.exe  --dbpath  "D:\MongoDB\data"   --journal  --storageEngine=mmapv1
 
4. 启动客户端 
mongo 192.168.0.24/test
