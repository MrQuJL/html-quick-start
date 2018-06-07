# html基础

## 什么是HTML

HTML（Hypertext Markup Language）即超文本标记语言。是用于描述网页文档的一种标记语言。就是用来写网页的，它不仅可以用来写文字还可以调整它的样式，所以就叫超文本，html 的内容由很多的标签组成（像这样：<p></p>），所以就叫超文本标记语言。

## 什么是HTML5

在 HTML 1,2,3,4 的基础之上又增加了一些更加炫酷的标签：canvas，svg，...etc。可以播放一些视频，音频，动画等。

## 什么是CSS

CSS（Cascading Style Sheets）即层叠样式表。使用来修饰 html 标签的，没有它，做出来的页面光秃秃的，不好看，有了 CSS ，HTML 就变得好看，原本光秃秃的 html 标签就有了样式，所以叫样式表。因为在下一行写的样式会覆盖前面相同类型的样式，所以叫层叠样式表。

## 什么是CSS3

在 CSS 的基础之上又添加了一些更炫酷的样式属性，例：圆角，阴影...etc。比 CSS 更好看了，所以叫 CSS3。

## 什么是Javascript

是一个客户端的脚本语言，可以让前台的标签动起来，就是你点按钮一下，他可以给你变个颜色，给你弹个提示框...etc。但是，你下次再请求一个页面的时候，还是原来的样子，应为它并没有去改变服务端的数据。如果你想与服务端交互也可以，用 jquery 封装好的 ajax 嘛。

## 使用editplus来编写页面（选择颜色）

* 这里推荐一款用来编写 html 的工具 -- editplus，非常好用，个人也是一直在用。

* 优点：不同的关键字有不同的颜色，干净，没有 Dreamweaver 那么多累赘的功能。最重要的一点，打开速度快！打开速度快！打开速度快！用 Dreamweaver 磨磨蹭蹭的卡半天，都想把电脑砸了。<br/>

* 缺点：功能没有 Dreamweaver 多（不过对于做后端的人来说基本用不上），没有 Dreamweaver 的代码提示多，倒是有标签的自动补全，例：写个 div ，按下 tab 键，就自动补全，其他的类似（个人觉得有这个就足够用了）。

## html模板配置

推荐个人一直在用的模板（**多用于自娱自乐，具体的规范看公司要求**）：

    <!doctype html>
    <html>
    <head>
        <meta http-equiv='Content-Type' content='text/html;charset=utf-8' />
        <title>模板</title>
        <meta name='keywords' content='关键词,关键词' />
        <meta name='description' content='网站描述' />
    </head>
    <body>
        <!-- 页面的html代码 -->
    </body>
    </html>


* ```<!doctype html>```：html5 的头标记。

* ```<html></html>```：里面放 html 主体。

* ```<head></head>```：html头部，多用于放一些页面加载时需要用到的css，js文件，若页面加载时不需要用到，就不要把css和js放到这里面，会影响页面的打开速度。

* ```<meta http-equiv='Content-Type' content='text/html;charset=utf-8' />```：页面编码utf-8。

* ```<title>模板</title>```：就是显示在浏览器选项卡上的标题。

* ```<meta name='keywords' content='关键词,关键词' />```：用于SEO，当你把网站发布到服务器上的时候，别人搜索一个关键词，就通过这个标记中的信息来查找到你的网页，所以现在有一个行业叫 SEO 优化，专门提升别人网站在百度的搜索排名。

* ```<meta name='description' content='网站描述' />```：就是百度快照中的内容。

* ```<body></body>```：在这里面写 html 代码。

## 单双标签的闭合方式

* 单标签：```<img />```, ```<input />```

* 双标签：```<div></div>```, ```<p></p>```

## 开发者工具箱F12的简易用法

打开方式：

    1. 右击 --> 检查
    2. 右击 --> 审查元素
    3. F12

![image](https://github.com/MrQuJL/html-quick-start/raw/master/01_html基础/imgs/box.png)

## css的写法（选择器）

    <head>
        <meta http-equiv='Content-Type' content='text/html;charset=utf-8' />
        <title>html基础</title>
        <meta name='keywords' content='关键词,关键词' />
        <meta name='description' content='网站描述' />
        <style type="text/css">
            *{margin:0;padding:0;}
            /*body{margin:0;}*/
            div{
                width:100px;
                height:100px;
                background:green;
                border:10px solid red;
                padding:20px;
            }
        </style>
    </head>

## js的写法

    ...
    <body>
    <script type="text/javascript">
        alert(1);
    </script>
    </body>
    ...

注：可以放在 body 里面，也可以放在 head 里面。

## border
    
    1. 多边框复合样式：
        border:1px solid red; /*边框大小 边框类型 边框颜色*/
    
    2. 多边框单样式:
        border-width:1px;
        border-style:solid;
        border-color:black;
    
    3. 单边框复合样式
        border-top:10px solid green;
        border-right:15px solid green;
        border-bottom:10px solid green;
        border-left:10px solid green;

    4. 单边框单样式：
        border-top-width:10px;
        border-top-style:solid;
        border-top-color:yellow;

    5. 边框类型：
        solid -- 实线
        dashed -- 虚线
        dotted -- 点线
        double -- 双横线

## padding

    1. 内边距：边框以内，内容以外
        padding:10px;
    
    2. 四个值：
        
        padding:5px 10px 15px 20px; /*上 右 下 左（顺时针）*/
        
        padding:5px 10px 15px; /*上 左右 下*/
        
        padding:5px 10px; /*上下 左右*/
        
        padding:5px; /*上下左右*/

    3. 一个方向的padding

        padding-top:10px;

        padding-right:10px;

        padding-bottom:10px;

        padding-left:10px;

## margin
    
    1. 外边距：边框与外面元素的距离
        margin:10px;
    
    2. 四个值：
        
        margin:5px 10px 15px 20px; /*上 右 下 左（顺时针）*/
        
        margin:5px 10px 15px; /*上 左右 下*/
        
		margin: 5px auto 10px; /*上 左右居中 下*/

        margin:5px 10px; /*上下 左右*/
        
		margin:5px auto; /*上下5px 左右居中*/

        margin:5px; /*上下左右*/

		margin:auto; /*左右居中*/

    3. 一个方向的margin

        margin-top:10px;

        margin-right:10px; /*距离右边如果很远则以较远的距离为准*/

        margin-bottom:10px; /*距离下边如果很远则以较远的距离为准*/

        margin-left:10px;

## 盒子大小的计算（重点）

**盒子的大小计算 = 内容大小（width height） + 内边距（padding） + 边框（border）**

## 宽高单位的另一种写法

```width:50%```：表示宽度为父级盒子的50%

## 颜色的几种表现形式

1. 英文颜色单词:blue

2. #十六进制颜色值:#ffffff，注：如果像上面这样每两个数字的值相同，可以两个变一个#fff，节省字节，加快页面的打开速度

3. rgb(0-255,0-255,0-255)
    255表示那个颜色的最大值

4. rgba(0-255,0-255,0-255,0-1)
    0表示完全透明
    1表示完全不透明

> 因为body默认有8个像素的外边距，导致div盒子不会紧贴浏览器，需要写如下代码来取消默认的外边距：

    body{margin:0;}

> 其他的标签也类似，所以我们在 css 样式的第一行统一加上这行代码来取消所有元素的外边距和内边距：

    *{margin:0;padding:0;}

## 练习

写一个 div盒子，要求如下：

* border 大小是 5 10 15 20 的盒子（用单样式写）

    ```html
    div{
        width:100px;
        height:100px;
        background-color:red;
        border-top-width:5px;
        border-right-width:10px;
        border-bottom-width:15px;
        border-left-width:20px;
        border-style:solid;/*不给边框加样式的话边框是显示不出来的*/
    }
    ```

* margin 大小是 20 15 10 5 的盒子（用单样式写）

    ```html
    div{
        width:100px;
        height:100px;
        background-color:red;
        margin-top:20px;
        margin-right:15px;
        margin-bottom:10px;
        margin-left:5px;
    }
    ```

* padding大小是 40 30 20 10的盒子（用单样式写）

    ```
    div{
        width:100px;
        height:100px;
        background-color:red;
        padding-top:40px;
        padding-right:30px;
        padding-bottom:20px;
        padding-left:10px;
    }
    ```
