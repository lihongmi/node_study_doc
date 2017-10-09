# 第2节 npm全局安装目录设置及镜像

1.
    修改 npm 模块的全局安装目录(npmrc文件)
        * prefix=d:\nodejs\node-global
        * cache=d:\nodejs\node-cache

    设置环境变量
    Path   


2.镜像

    npm 的官方镜像是非常慢

    我们可以使用淘宝定制的 cnpm (gzip 压缩支持) 命令行工具代替默认的 npm

    * npm install -g cnpm --registry=https://registry.npm.taobao.org
    * cnpm install xxx

    或者 修改npmrc文件
    registry = https://registry.npm.taobao.org


3.nrm -- NPM registry 管理工具

    *  安装
    npm install -g nrm

    * 使用

    nrm ls
    nrm use cnpm

4.yarn 包管理工具

    * https://yarnpkg.com/en/docs/install
    * https://yarn.bootcss.com/docs/getting-started.html


