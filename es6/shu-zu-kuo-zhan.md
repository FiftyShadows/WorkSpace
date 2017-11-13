##数组新增特性

- Array.from

- Array.of

- copyWithin

- find\findIndex

- fill

- entries\keys\values

- includes



##Array.of把一组数据变量转换成数据类型

```
{
    let arr = Array.of(3,4,7,9,11);
    console.log('arr = ',arr);    //arr = [3,4,7,9,11]
    
    let empty = Array.of();
    console.log('empty', empty);    //empty[]
}
```


##Array.form

1. 把一些伪数组或集合转换成真正的数组

2. 类似于map的映射

```
{
    let p = document.querySelectorAll('p');
    let pArr = Array.from(p);
    pArr.forEach(function(item){
        console.log(item.textContent);
    });
    
    
    console.log(Array.from([1,3,5], function(item){return item*2}));    //[2,6,10]
    
}
```


##fill

1. 填充数组，把数组所有元素换成一个值

```
{
    console.log('fill-7', [1, 'a', undefined].fill(7));    //[7,7,7]
}
```


2. 

```
{
    console.log('fill,pos', ['a', 'b', 'c'].fill(7,1,3));    //[7,7,7]
}
``




































