# 第1节  npm包的相关命令


nodejs的包管理工具

>npm 有上万的包 发布在  http://www.npmjs.org/



安装完node 建议  升级 npm 包管理工具

npm i -g npm



常见的npm命令


npm init  产生一个  package.json

列出已安装依赖
* npm list -g
* npm list 显示你已经安装过的包


安装
* npm install  xxx -gd
* npm install  xxx --save-dev

卸载
* npm unstall  xxx -gd  
* npm unstall  xxx

升级
* npm update  xxx -gd  
* npm update  xxx

查询及查看包的所有版本
* npm search xxx
* npm view xxx versions

npm root 查看依赖安装路径

* npm root -g


npm view 查看模块的注册信息

* xxx versions 列出xxx的所有版本， 如：npm view jquery versions。
* xxx dependencies 列出xxx的所有依赖， 如：npm view gulp dependencies。


