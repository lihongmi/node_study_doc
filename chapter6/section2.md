# 第2节 mongodb安装

mongodb
 是一款 nosql 数据库  
 
面向文档(collection)的数据库
存储数据格式 bson

1.mongodb的安装
---

2.创建数据目录
 data/db

3.启动mongodb服务器
mongod.exe --dbpath D:\MongoDB\data\db

4.启动客户端 
mongo 192.168.0.24/test

5.插入数据

db.student.insert({name:"redrice",age:31,sex:1});
db.student.insert({name:"jiayunzhe",age:21,sex:1});
db.student.insert({name:"liuhui",age:23,sex:0});


6.查询 数据
db.student.find({sex:1})

7.修改数据
 db.student.update({name:"jiayunzhe"},{$set:{age:26}})

8.删除数据
 db.student.remove({name:"redrice"});