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



















