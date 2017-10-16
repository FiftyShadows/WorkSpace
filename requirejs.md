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


























































