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

![](/assets/360截图20171017110618448.jpg)

![](/assets/360截图20171017110701608.jpg)

![](/assets/360截图20171017132728771.jpg)





##指令

- 在指令里操作DOM（link）

![](/assets/360截图20171017133718392.jpg)


- 独立scope

![](/assets/360截图20171017144844105.jpg)

![](/assets/360截图20171017145011097.jpg)


- @

![](/assets/360截图20171017145205348.jpg)

![](/assets/360截图20171017145220209.jpg)

![](/assets/360截图20171017145419799.jpg)




- =双向绑定

![](/assets/360截图20171017145740184.jpg)

![](/assets/360截图20171017145707799.jpg)



- &

![](/assets/360截图20171017150146523.jpg)

![](/assets/360截图20171017150203475.jpg)


####内置的指令

![](/assets/360截图20171017150739129.jpg)

![](/assets/360截图20171017150944648.jpg)

![](/assets/360截图20171017151401990.jpg)

![](/assets/360截图20171017151622357.jpg)


AngularUI第三方指令库

![](/assets/360截图20171017153047109.jpg)


Kissy Gallery









