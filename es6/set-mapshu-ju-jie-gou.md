  ##数据结构
  
  - Set的用法
  
  - WeakSet的用法
  
  - Map的用法
  
  - WeakMap的用法
  
***set（可当做数组）集合中的元素是不能重复的,map（跟object作对比，key是字符串）key可以是任意的数据类型***


##Set

- 用add方法给Set里面增加元素

- size方法获取变量有几个元素

```
{
  let list = new Set();
  list.add(5);
  list.add(7);
  console.log('size', list.size);
}

{
  let arr = [1, 2, 3, 4, 5];
  let list = new Set(arr);
}
```



