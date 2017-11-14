##Symbol的概念

- 这种数据类型提供一个独一无二的值（这种方式声明的变量的值永远都不会相等）

```
{
    //声明
    let al = Symbol();
    let a2 = Symbol();
    console.log(a1 === a2);    //false
    
    //Symbol.for(key值)，有key值的时候，会检查全局是否注册过，注册过返回值，没注册过调Symbol生成一个独一无二的值
    let a3 = Symbol.for('a3');
    let a4 = Symbol.for('a3');
    console.log(a3 === a4);    //true
}
```


##Symbol的作用

```
{
    let a1 = Symbol.for('abc');
    let obj = {
        [a1]: '123',
        'abc': 345,
        'c': 456
    }
    consolo.log('obj', obj);
    
    for(let [key, value] of Object.entries(obj)){
        console.log('let of', key, value);    取不到[a1]
    }
    
    Object.getOwnPropertySymbols(obj).forEach(function(item){
        console.log(obj[item]);    //123
    })
    
    Reflect.ownKeys(obj).forEach(function(){
    
    })
}
```

######注意

- 对象中有用到Symbol做key值，通过for...in和let...of拿不到该属性

- Object.getOwnPropertySymbols能取到Symbol属性的值

- Reflect.ownKeys(obj)包含了Symbol变量作为key值的属性，也包含了非Symbol变量的属性








