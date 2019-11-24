# 子元素选择器



## :first-child

选中第一个子元素，如果在选中元素之前加一个别的标签，则选择失效

```html
<style>
        p:first-child{
            background-color: yellow;
        }
</style>
<body>
    
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>

</body>
```



效果：

![](https://i.loli.net/2019/11/23/Yrw9FxRvqHy3BUt.png)

这样写，不会考虑你是考虑你是哪一个元素的子元素，只要你是子元素且是p标签就行

例如:

```html
    <div>
        <p>我是一个段落</p>
    </div>
```

这样里面的p标签也是会变成黄色的，因为同样符合条件，如果想显示一个p元素的话，应该如下

```html
<style>
        body > p:first-child{
            background-color: yellow;
        }
</style>
```

这样就会选中，body的第一个子元素 p



## :last-child

选中最后一个子元素，特性与**first-child**一样

```html
<style> 
        p:last-child{
                    background-color:red;
        }
</style>
<body>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
</body>
```

效果：

![](https://i.loli.net/2019/11/24/fw85m1ChZpoXjDa.png)





## :nth-child(参数)

选中第n个子元素

```html
<style> 
        p:nth-child(3){
            background: blue;
        }
</style>
<body>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
</body>
```

效果：

![](https://i.loli.net/2019/11/24/xSygCHbLEUAzY3M.png)

括号里面还可以设置特殊值，例如: even（偶数）、odd（基数）

```html
<style> 
        p:nth-child(odd){
            background: blue;
        }
</style>
```

效果：

![](https://i.loli.net/2019/11/24/6GxMb3fyrcXL8Wq.png)





## :first-of-type、last-of-type、nth-of-type

用法和child一样，用于查找当前类型的子元素

```html
<style> 
        p:first-of-type{
            background-color: orange;
        }
</style>
<body>
    <span>我是一行</span>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
</body>
```

效果：

![](https://i.loli.net/2019/11/24/n7qV9G3CRTofiU8.png)

