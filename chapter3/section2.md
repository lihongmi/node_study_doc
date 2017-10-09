# 第2节 模块的定义与引用

* 模块的定义第一种方法

``` javascript

    exports.s=mianji;
    exports.l=zhouchang;
    exports.ABC=21;
```

* 模块的定义第二种方法

```javascript
    module.exports={
        s:mianji,
        l:zhouchang,
        ABC:21
    };
```

*   require("");

