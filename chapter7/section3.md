# 第3节 mongodb  数据操作命令

show dbs;

use student;

db.stats()

show collections;







1.插入数据

db.student.insert({name:"redrice",age:31,sex:1});
db.student.insert({name:"jiayunzhe",age:21,sex:1});
db.student.insert({name:"liuhui",age:23,sex:0});

2.查询 数据
db.student.find({sex:1})

3.修改数据
 db.student.update({name:"jiayunzhe"},{$set:{age:26}})

4.删除数据
 db.student.remove({name:"redrice"});