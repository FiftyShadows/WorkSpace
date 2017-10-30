1. template parse errors

![](/assets/360截图20171023164722902.jpg)

![](/assets/360截图20171023164859716.jpg)



2. Can't bind to 'formControl' since it isn't a known property of 'input'. ("">

![](/assets/360截图20171024191429386.jpg)

为了能够在表单输入中使用双向数据绑定，主模块中导入FormsModule。








Angular使用less管理css样式

首先我们需要修改angular-cli.json中的配置信息
```
 "apps": [
    {
      "styles": [
        "styles.less"
      ]  
  ],
  "defaults": {
    "styleExt": "less",
  }
```

由于改变了Angular的配置中的css为less,因此 你所有的css后缀文件都要改成less。

































