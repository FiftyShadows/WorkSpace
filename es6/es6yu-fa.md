##函数新增特性

- 简洁表示法

- 属性表达式

- 扩展运算符

- Object新增方法


##简洁表示法

```
{
    let o = 1;
    let k = 2;
    let es5 = {
        o: o,
        k: k
    };
    let es6 = {
        o,
        k
    };
    console.log();
    
    //方法
    let es5_method = {
        hello: function(){
            console.log('hello');
        }
    };
    let es6_method = {
        hello(){
            console.log('hello');
        }
    };
    console.log(es5_method.hello(), es6_method.hello());
}
```


##属性表达式

```
{
    let a = 'b';
    let es5_obj = {
        a: 'c'
    };
    
    let es6_obj = {
        [a]: 'c'    //这里的a是一个表达式，相当于b: 'c'
    }
    console.log(es5_obj, es6_obj);
}
```


##Object新增方法

```
{
    console.log('字符串', Object.is('abc', 'abc'), 'abc' === 'abc');
}
```







































