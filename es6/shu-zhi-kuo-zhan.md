## 二进制数值的表示方法

```
{
    console.log('0b111110111');
    console.log(''0B111110111');
}
```

## 

## 八进制表示

```
{
    console.log('0o767');
    console.log('0O767');

}
```

## 

## 判断一个值是否有尽Number.isFinite

```js
{
     console.log('15',Number.isFinite(15));//true
     console.log('NaN',Number.isFinite(Nan)); //false
     console.log('1/0',Number.isFinite('true'/0));//false
}
```

## 

## 判断是不是非数字Nimber.isNaN

`console.log('0',Number.isNan(0));//false`

## 

## 判断是不是整数Number.isInteger

`console.log('25.0',Number.isInteger(25.0));//true`  
`console.log('25',Number.isInteger('25'));//false`

##

##判断一个数是否在$-2^53=$到$2^53$

####两个常量

最大上限`console.log(Number.MAX_SAFE_INTEGER);`


最小下限`console.log(Number.MIN_SAFE_INTEGER);`

####判断一个数是否安全Number.isSafeInteger

`console.log('10',Number.isSafeInteger(10));//true`

`console.log('a',Number.isSafeInteger('a'))    //false;`


##判断带小数的整数部分，并返回Math.trunc

`console.log(4.1, Math.trunc(4.1));    //4`


##判断一个数是正数，负数，还是0 Math.sign

```
{
    console.log('-5', Math.sign(-5));    //-1
    console.log('0', Math.sign(0));    //0
    console.log('5', Math.sign(5));    //1
    console.log('50', Math.sign('50'));    //1
    console.log('foo', Math.sign('foo'));    //NaN
}
```


##立方根的计算Math.cdrt

`console.log('-1',Math.cbrt(-1));    -1`














