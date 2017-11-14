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
        
    }
    console.log('继承', new Child());
}
```



























