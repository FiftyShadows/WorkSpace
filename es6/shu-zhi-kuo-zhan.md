##二进制数值的表示方法

```
{
    console.log('0b111110111');
    console.log(''0B111110111');
}
```


##八进制表示

```
{
    console.log('0o767');
    console.log('0O767');

}
```


##判断一个值是否有尽Number.isFinite

```js
{
     console.log('15',Number.isFinite(15));//true
     console.log('NaN',Number.isFinite(Nan)); //false
     console.log('1/0',Number.isFinite('true'/0));//false
}
```


##判断是不是非数字Nimber.isNaN
`console.log('0',Number.isNan(0));//false`



##判断是不是整数Number.isInteger
`console.log('25.0',Number.isInteger(25.0));//true`







