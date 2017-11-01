##const和let是块作用域使用的变量类型

- let声明的变量只在自己的块内有效，不能重复定义变量

- const声明时必须赋值

![](/assets/360截图20171101210551899.jpg)

这里const声明了对象，对象是引用类型，K存储的是对象的地址，修改对象不会改变地址。




##解构赋值

- 解构赋值的分类：数组解构赋值，对象解构赋值，字符串解构赋值，布尔值解构赋值，函数参数解构赋值，数值解构赋值

- 数组解构赋值

![](/assets/360截图20171101211402874.jpg)

![](/assets/360截图20171101211459459.jpg)

- 对象解构赋值

![](/assets/360截图20171101211745337.jpg)

![](/assets/360截图20171101212040778.jpg)

如果解构赋值没有在结构上成功配对，没有配对的变量为    undefined

####解构赋值的使用场景

- 变量交换

![](/assets/360截图20171101212203098.jpg)

- 获取函数返回值

![](/assets/360截图20171101212325367.jpg)

- 获取函数某些返回值

![](/assets/360截图20171101212441277.jpg)

- 返回值个数不确定时

![](/assets/360截图20171101212550779.jpg)


![](/assets/360截图20171101215015078.jpg)





##正则扩展

- 正则新增特性:构造函数的变化、正则方法的扩展、u修饰符、y修饰符、s修饰符






















