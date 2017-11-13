##函数新增特性

- 参数默认值

- rest参数

- 扩展运算符

- 箭头函书

- this绑定

- 尾调用



##参数默认值

```
{
    function test(x, y = 'world'){
        console.log('默认值', x, y);
    }
    test('hello');
    test('hello', 'kill');
}
```



```
{
    let x = 'test';
    function test2(x, x = y){
        console.log('作用域', x, y);
    }
    test2('kill');    //作用域 kill kill
    test2();    //作用域 undefined undefined
}
```



















