# 伪类选择器



## :first-letter

为元素第一个字符设置样式

```html
<style>
         p:first-letter {
            color: red;
            font-size: 20px;
        } 
</style>

<body>
    <p>这是一个段落</p>
</body>

```

效果：

![](https://i.loli.net/2019/11/23/ReHIfv6P7jLqo8E.png)



## :first-line

为元素的第一行设置样式

```html
<style>

        p:first-letter {
            color: red;
            font-size: 20px;
        }

        p:first-line {
            background-color: yellow;
        }

</style>

<p> “魏无羡死了。大快人心！”
    乱葬岗大围剿刚刚结束，未及第二日，这个消息便插翅一般飞遍了整个修真界，比之当初战火蔓延的速度有过之而无不及。
        一时之间，无论是世家名门，还是山野散修，人人都在议论此次由四大玄门世家联率、大小百家参与混战的围剿行动。
</p>
```





效果：

![](https://i.loli.net/2019/11/23/qSyx35WfjzQbAN9.png)





## :before

before代表元素最前面的部分，一帮与**content**样式一起使用，通过**content**可以向其中添加内容，否则会不显示任何东西

```html
<style>
        p:before{
            color:red;
            content:"我出现在段落最前面";
        }
</style>

<p> “魏无羡死了。大快人心！”
    乱葬岗大围剿刚刚结束，未及第二日，这个消息便插翅一般飞遍了整个修真界，比之当初战火蔓延的速度有过之而无不及。
        一时之间，无论是世家名门，还是山野散修，人人都在议论此次由四大玄门世家联率、大小百家参与混战的围剿行动。
</p>
```

效果：

![](https://i.loli.net/2019/11/23/8f7sXkdIoiVymcD.png)





## :after

表示元素后面的部分，用法和before一样

```html
<style>
        p:after{
            color:orange;
            content:"我出现在段落最后面";
        }
</style>

<p> “魏无羡死了。大快人心！”
    乱葬岗大围剿刚刚结束，未及第二日，这个消息便插翅一般飞遍了整个修真界，比之当初战火蔓延的速度有过之而无不及。
        一时之间，无论是世家名门，还是山野散修，人人都在议论此次由四大玄门世家联率、大小百家参与混战的围剿行动。
</p>
```



效果：

![](https://i.loli.net/2019/11/23/Ja5ANDkBbmz6OEY.png)



