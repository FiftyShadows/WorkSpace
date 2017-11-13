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


2. 替换部分数值fill(要替换得值，起始位，结束位) 

```
{
    //从1号位置，到3号位置
    console.log('fill,pos', ['a', 'b', 'c'].fill(7,1,3));    //[7,7,7]
}
``


##entries\keys\values

```js
{
    //返回数组的下标，of后边[0, 1, 2]
    for(let index of ['1', 'c', 'ks'].keys()){
        console.log('keys', index);
    }
    
    //返回数组的值(需要bebel-polyfill兼容)
    for(let index of ['1', 'c', 'ks'].values()){
            console.log('keys', index);
    }
    
    
    for(let [index, value] of ['1', 'c', 'ks'].entires()){
        console.log('entries', index, value);
    }
}
```


##copyWithin(从哪个位置开始替换， 从哪个位置开始读取数据， 从哪个位置截止)

```
{
    console.log([1, 2, 3, 4, 5].copyWithin(0, 3, 4));    //[4, 2, 3, 4, 5]
}
```


##find\findIndex

- find只找到第一个符合的值，便不再往后找了

- findIndex找到第一个符合条件的值得下标

- includes数组是否包含某个值


```
{
    console.log([1, 2, 3, 4, 5, 6].find(function(item){return item > 3}));    //4
    
    console.log([1, 2, 3, 4, 5, 6].findIdex(function(item){return item > 3}));    //3
}

    console.log('number', [1, 2, NaN] .includes(1));    //true
    console.log('number', [1, 2, NaN] .includes(NaN));    //true
```
































