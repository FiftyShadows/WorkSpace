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















