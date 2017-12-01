## 同步实现A执行完执行B

1. 回调

2. 事件触发

回调的方式：1.复杂；2.难以维护

## 

## 

## Promise

![](/assets/360截图20171113143351561.jpg)

![](/assets/360截图20171113152805136.jpg)

### 

### 

#### promise.all\(\[\]\).then\(\)

* 所有图片都加载完再添加到页面

```js
{
//所有图片都加载完再添加到页面
    function loadImg(src){
        return new Promise((resolve,reject) => {
            let img = document.createElement("img");
            img.src = src;
            img.onload = function(){
                resolve(img);
            }
            img.onerror = function(){
                reject(err);
            }
        })
    } 


    function showImgs(imgs){
        imgs.forEach(function(img){
            document.body.appendChild(img);
        })
    }


    Promise.all([
        loadImg('https://unsplash.it/320/150/?random'),
        loadImg('https://unsplash.it/320/150/?random'),
        loadImg('https://unsplash.it/320/150/?random')
    ]).then(showImgs)


}
```

* 有一个图片加载完就添加到页面

```
{
    function loadImg(src){
        return new Promise((resolve,reject) => {
            let img = document.createElement("img");
            img.src = src;
            img.onload = function(){
                resolve(img);
            }
            img.onerror = function(){
                reject(err);
            }
        })
    }

    function showImgs(img){
        let p = document.createElement("p");
        p.appendChild(img);
        document.body.appendChild(p);
    }

    Promise.rase([
        loadImg('https://unsplash.it/320/150/?random'),
        loadImg('https://unsplash.it/320/150/?random'),
        loadImg('https://unsplash.it/320/150/?random')        
    ]).then(showImgs)


}
```



