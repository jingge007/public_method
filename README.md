# public_method.js (对一些常用js的公共方法的总结与归纳)

## public_method 介绍

`public_method.js`  是自己在平时开发中常用到的一些js方法的整理与总结，因为平时开发中我们会用到各种各样的公共方法去处理不同的数据，
所以我就在这里整理以前自己开发中常用的一些方法，当做插件使用避免我们开发中要不断的去写这些方法，又繁琐开发效率也不高。

## public_method 的使用方法

`public_method` 的使用方法相当的简单与便捷，这里我对  `public_method`  的封装是采用了Javascript模块化编程的对象写法。
把定义好的公共方法都放到 `pubilc` 对象中，然后在页面上调用的时候就直接引用 `public_method.js` 文件通过public对象调用
不同的公共方法。 

例如：在html页面中使用
```js
<script src="js/public_method.js"></script>
<script>
    let timer = 620;
    pubilc.timer_format(timer)   // 这里就是调用pubilc对象中的timer_format的公共方法，只需要把对应的参数传给公共方法就行了
</script>
```


例如：在vue中使用
```vuejs
在main.js中或者在组件中引入public_method.js文件
import 'common/js/public_method' 然后就可以全局引用或者在对应的组件中使用了
```
## end 

`public_method.js` 是自己的一些js常用的方法的整理与总结，多多少少肯定都有一些地方写的不好，如果那里写的不好的
希望小伙伴们可以指出问题，大家相互学习，共同进步！！！如果小伙伴们也有好的公共方法可以分享一波，也可以添加到 `public_method.js` 
大家都可以共同维护，如果你觉得 `public_method` 还不错可以 `star` 一波给个星星，也可以 `followers` 关注一波！！！


