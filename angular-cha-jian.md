##angular-async-loader

####传统的 angular 应用不支持异步加载模块，必须在 module 启动的时候，所有模块必须预加载进来。 通过使用 angular-async-loader 库，我们可以使用 requirejs 等加载器，在 module 初始化之后，在动态异步加载其他的 Controller, Services, Filters 等等......




##angular-ui-router



##ngDialog

```
$scope.del = function () {  
            ngDialog.open({  
                template: '/del.html',  
                className: 'ngdialog-theme-default',  
                scope: $scope,  
                controller: function ($scope) {  
                ...  
                    $scope.confirm = function () {  
                    ...  
                    };  
                    $scope.cancel = function () {  
                        $scope.closeThisDialog();  
                    };  
                }  
          });  
}; 
```




##angular-cookies

在App 中require模块ngCookies---------angular.module("app",['ngCookies']);
使用格式：$cookies.变量名 = 变量值
不能使用：$cookies.变量名 = {
变量名1： 变量值，
变量名2： 变量名，
.............
}
因为这样使用：$cookies.变量名.变量名1的方式就不被识别

cookies存储少量数据
cookieStore采用key-value(String-object)方式存储数据,
put,get,remove分别用于存数据，取数据，移除数据

```
angular.module('cookieStoreExample', ['ngCookies'])
  .controller('ExampleController', ['$cookieStore', Function($cookieStore) {
    // Put cookie
    $cookieStore.put('myFavorite','oatmeal');
    // Get cookie
    var favoriteCookie = $cookieStore.get('myFavorite');
    // Removing a cookie
    $cookieStore.remove('myFavorite');
  }]);
```

可以以对象的形式存储

`$cookieStore.put("user",{id: "id",name: "name"});`




##angular-file-upload

`<input type="file" nv-file-select uploader="uploader"/>`

前面的file是input上传时用的特殊type，nv-file-select 是上传的样式，这个是最近基本的文件上传，还有nv-file-over这个是拖动到指定位置上传 nv-file-drop这个你直接把文件拖进网页就可以上传。

后面的uploader="uploader"这个也是必填的 ，这个是我们实例一个上传实例，你可以看到我们的controller有$scope.uploader = new FileUploader();这就是实例一个上传，我们前台得到这个实例，然后操作。

两个属性是必须的，还有两个可选属性options="{Object}" filters="{String}" 

```
uploader.filters.push({
        name: 'customFilter',
        fn: function(item, options) {
            return this.queue.length < 10;
        }
    });
```

过滤器的名字是customFilter 方法执行子fn里 queue是文件上传实例也就是uploader的属性


```
var uploader = $scope.uploader = new FileUploader({
        url: 'http://localhost:8080/服务器',
    });
```
