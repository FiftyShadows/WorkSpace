##require.config()方法

- require.config()就写在主模块（main.js）的头部。参数就是一个对象，这个对象的paths属性指定各个模块的加载路径。


```
require.config({
　　　　baseUrl: "js/lib",
　　　　paths: {
　　　　　　"jquery": "jquery.min",
　　　　　　"underscore": "underscore.min",
　　　　　　"backbone": "backbone.min"
　　　　        }
　　        });
```


##加载非规范的模块

- exports值（输出的变量名），表明这个模块外部调用时的名称；

- deps数组，表明该模块的依赖性。


```js
require.config({
　　　　shim: {

　　　　　　'underscore':{
　　　　　　　　exports: '_'
　　　　　　            },
　　　　　　'backbone': {
　　　　　　　　deps: ['underscore', 'jquery'],
　　　　　　　　exports: 'Backbone'
　　　　　　            }
　　　　        }
　　            });
```





##require.js插件

- domready插件，可以让回调函数在页面DOM结构加载完成后再运行。

- text和image插件，则是允许require.js加载文本和图片文件。

- 类似的插件还有json和mdown，用于加载json文件和markdown文件。
















































