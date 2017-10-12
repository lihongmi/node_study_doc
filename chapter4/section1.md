# 第1节 http https模块

一. http
---
1. http.createServer
    .listen

    res 响应  req  请求

    res.end
    res.write

    req.url


2. http.request

https 需要 SSL证书


二. https
---

cygwin

* 私钥key文件
openssl genrsa -out privatekey.pem 1024
* CSR证书签名
openssl req -new -key privatekey.pem -out certrequest.csr
* 私钥和证书签名生成证书文件
openssl x509 -req -in certrequest.csr -signkey privatekey.pem -out certification.pem



``` javascript
   const https = require('https');
    const fs = require('fs');

    const options = {
        key: fs.readFileSync('./privatekey.pem'),
        cert: fs.readFileSync('./certification.pem')
    };

    https.createServer(options, (req, res) => {
        res.writeHead(200);
        res.end('hello world\n');
    }).listen(8000);
```
