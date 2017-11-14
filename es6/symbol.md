##Symbol的概念

- 这种数据类型提供一个独一无二的值（这种方式声明的变量的值永远都不会相等）

```
{
    //声明
    let al = Symbol();
    let a2 = Symbol();
    console.log(a1 === a2);    //false
    
    let a3 = Symbol.for('a3');
    let a4 = Symbol.for('a3');
    console.log(a3 === a4);    //true
}
```

##Symbol的作用


