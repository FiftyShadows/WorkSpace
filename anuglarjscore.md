##angular-route不能深层次嵌套路由

angular-ui-router来实现

ui-view显示多视图

```
    $urlRouterProvider.otherwise("/index");

    //dependencies: ['services/usersService']
    $stateProvider.state('index', {
        url: '/index',
        templateUrl: 'html/index/index.html',
        controllerUrl: 'controllers/indexCtrl',
        controller: 'indexCtrl',
    })
```

























































