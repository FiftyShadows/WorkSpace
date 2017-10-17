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








##MVC

![](/assets/360截图20171017004250713.jpg)

![](/assets/360截图20171017004323275.jpg)

![](/assets/360截图20171018015306582.jpg)

AngularJS的MVC是借助于$scope实现的！






##双向数据绑定

![](/assets/360截图20171018003149368.jpg)

`ng-class="{active: type == 'local'}"`

开关效果

![](/assets/360截图20171018004927640.jpg)






##指令

![](/assets/360截图20171017005328673.jpg)

![](/assets/360截图20171017005650340.jpg)

- replace:true;替换

- transclude:true;将你的指令内部的元素（注意不是指令的模板）嵌入到你的模板中去

![](/assets/360截图20171017235516304.jpg)

![](/assets/360截图20171017005717001.jpg)




####指令的三个阶段

![](/assets/360截图20171017010207515.jpg)

- link绑定事件

![](/assets/360截图20171017011010698.jpg)

![](/assets/360截图20171017011215921.jpg)

- 什么时候逻辑写在controller里，什么时候写在link里？

要向外部暴露一些方法让web调用就写在controller里，link处理指令内部的事物，给元素绑定事件或数据。

![](/assets/360截图20171018002013021.jpg)

![](/assets/360截图20171018002028187.jpg)





- 独立scope

![](/assets/360截图20171018002741127.jpg)

没有独立scope，会影响到其他三个指令的数据

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

![](/assets/360截图20171018003005085.jpg)

![](/assets/360截图20171017150944648.jpg)

![](/assets/360截图20171017151401990.jpg)

![](/assets/360截图20171017151622357.jpg)


AngularUI第三方指令库

![](/assets/360截图20171017153047109.jpg)


Kissy Gallery






##service和provider

![](/assets/360截图20171017164640527.jpg)

![](/assets/360截图20171017171148370.jpg)

![](/assets/360截图20171017172020462.jpg)

![](/assets/360截图20171017172458304.jpg)

![](/assets/360截图20171017172731394.jpg)

自定义filter

![](/assets/360截图20171017173412086.jpg)

![](/assets/360截图20171017173747421.jpg)






##综合应用

![](/assets/360截图20171017174449020.jpg)



















































