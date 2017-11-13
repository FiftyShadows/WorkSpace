回调的方式：1.复杂；2.难以维护

## 

## 

## Promise

![](/assets/360截图20171113143351561.jpg)

### 

### 

#### promise.all([]).then()

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
        loadImg('https://unsplash.it/320/150/?random');
        loadImg('https://unsplash.it/320/150/?random');
        loadImg('https://unsplash.it/320/150/?random');
    ]).then()


}
```

