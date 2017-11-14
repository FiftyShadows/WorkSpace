  ##数据结构
  
  - Set的用法
  
  - WeakSet的用法
  
  - Map的用法
  
  - WeakMap的用法
  
***set（可当做数组）集合中的元素是不能重复的,map（跟object作对比，key是字符串）key可以是任意的数据类型***


##Set

- 用add方法给Set里面增加元素

- size方法获取变量有几个元素


```js
//第一种定义方式
{
  let list = new Set();
  list.add(5);
  list.add(7);
  console.log('size', list.size);  //size 2
}

//第二种定义方式
{
  let arr = [1, 2, 3, 4, 5];
  let list = new Set(arr);
  console.log('size', list.size);  //size 5
}
```


- 唯一性去重,不会做数据类型转换

```
{
   let list = new Set();
   list.add(1);
   list.add(2);
   list.add(1);  //不会报错，但不生效
   console.log('list', list);
   
   let  arr = [1, 2, 3, 1, '2'];
   let list2 = new Set(arr);
   console.log('unique', list2);  //unique Set{1, 2, 3, '2'}
}
```

- delete, clear, has

```
{
  let arr = ['add', 'delete', 'clear', 'has'];
  let list = new Set(arr);
  console.log('has', list.has('add'));  //has true 
  console.log('');
}
```






