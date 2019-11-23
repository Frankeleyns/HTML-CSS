# 属性选择器
作用：可以根据元素中的属性或属性值来选取指定元素



## [属性名]

选取含有**指定属性**的元素


```html
<style>
    /*
    * 选中所有具有title属性的p元素
    */
    p[title]{
        background-color: yellow;
    }
    
</style>

<body>

        <p title="hello">我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p title="abc">我是一个段落</p>
        
</body>
```

效果：

![](https://i.loli.net/2019/11/23/dU5D7Z8uNFoh2On.png)



## [属性名 = “属性值” ]

选取含有**指定属性值**的元素

```html
<style>
    p[title = "hello"]{
        background-color: red;
    }
</style>

<body>

        <p title="hello">我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p title="abc">我是一个段落</p>

</body>
```

效果：

![](https://i.loli.net/2019/11/23/f3Qtg6uvEwBCLGh.png)





## [属性名 ^= “属性值” ]

选取属性值以指定内容**开头**的元素

```html
<style>
    p[title ^= "abc"]{
        background-color: blue;
    }
</style>

<body>

        <p title="hello">我是一个段落</p>
        <p title="abc">我是一个段落</p>
        <p title="abce">我是一个段落</p>
        <p title="bbcd">我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>

</body>
```

效果：

![](https://i.loli.net/2019/11/23/l2fiOydmaNpBxo4.png)



## [属性名 $= “属性值” ]

选取属性值以指定内容**结尾**的元素

```html
<style>
    p[title $= "c"]{
        background-color: orange;
    }
</style>
<body>

        <p title="helloc">我是一个段落</p>
        <p title="abc">我是一个段落</p>
        <p title="abce">我是一个段落</p>
        <p title="bbcd">我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>

</body>
```

效果：

![](https://i.loli.net/2019/11/23/ya4IKTx9s6jXtwN.png)





## [属性名 *= “属性值” ]

选取属性值以**包含**指定内容的元素

```html
<style>
    p[title *= "c"]{
        background-color: green;
    }
</style>
<body>

        <p title="helloc">我是一个段落</p>
        <p title="abc">我是一个段落</p>
        <p title="abce">我是一个段落</p>
        <p title="bbcd">我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>
        <p>我是一个段落</p>

</body>
```

效果：

![](https://i.loli.net/2019/11/23/7btrHndVxAZ2CJa.png)