##类

- 基本语法

- 类的继承

- 静态方法

- 静态属性

- getter

- setter



##基本语法

```
{
    class Parent{
        constructor(name = 'imooc'){
            this.name = name;
        }
    }
    let v_parent = new Parent('v');
    console.log('构造函数和实例', v_parent);
}
```



##继承

```
{
    class Parent{
        constructor(name = 'imooc'){
            this.name = name;
        }
    }
    class Child expends Parent{
        constructor(name = 'child'){
            super(name);
            this.type = 'child';    //super要放在构造函数第一行
        }
    }
    console.log('继承', new Child());
    console.log('继承传递参数', new Child('hello'));
}
```


##getter

```
{
    class Parent{
        constructor(name = 'imooc'){
            this.name = name;
        }
        get longName(){    //这里是属性，不是方法
            return 'mk' + this.name
        }
        set longName(value){
            this,name = value;
        }
    }    
}
```
























