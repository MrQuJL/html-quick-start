# 常用标签及属性

## div（最常用）

块级标签

    <div></div>

## img（图片标签）

    <img src="hibernate.jpg" alt="seo" title="标题" width="200px" height="200px" />

* src：指定文件的位置。

* width：规定宽度 如果只规定宽度后，图片等比例缩放。

* height：规定高度 如果只规定高度后，图片等比例缩放。

* title：鼠标划上去的时候显示的文字（利于用户体验）。

* alt：用于SEO，在百度搜索:"图片 比亚迪"，能够出现比亚迪图片就是因为这个属性，可以使百度蜘蛛能够抓取到这个图片。

## a（超链接标签）

> 默认样式：字体蓝色，带下划线。

* href：连接到的网页的 url，如果 url 中是一个文件（pptx）还可以实现下载

    ```
    <a href="xxx.pptx">下载</a>
    ```

* href：还可以用来当锚点，跳转到指定id的标签的位置（用于在页面很长的情况下，进行页面间跳转，例：返回顶部）

    ```
    <a href="#item4">锚点</a>

    <ul>
        <li id="item1"></li>
        <li id="item2"></li>
        <li id="item3"></li>
        <li id="item4"></li>
    </ul>
    ```

* target：网页打开的位置，共两个值：_blank(在一个空白页打开),_self(替换当前页面 - 默认) 

    <a href="https://www.baidu.com" target="_blank">a标签</a>

## base

> 用来定义超链接默认的打开方式(target)，放在 head 标签里面。

    <head>
        <meta http-equiv='Content-Type' content='text/html;charset=utf-8' />
        <base target="_blank">
        <title>各种标签</title>
        <meta name='keywords' content='关键词,关键词' />
        <meta name='description' content='网站描述' />
    </head>

## h1 ~ h5（标题标签）

> 为了利于SEO，h1标签建议只在页面上使用一次

    <h1>h1标题标签</h1>

    <h2>h2标题标签</h2>

    <h3>h3标题标签</h3>

    <h4>h4标题标签</h4>

    <h5>h5标题标签</h5>

## p（段落标签）

> 主要用于放一些文字（放屁）

## span（行内标签）

> 可以在一行显示多个 span 标签的内容

## ul li（无序列表）

> li 前面是小圆点

    <ul>
        <li>item1</li>
        <li>item2</li>
        <li>item3</li>
        <li>item4</li>
    </ul>

* 主要用于做一些导航：像天猫的：

![image](https://github.com/MrQuJL/html-quick-start/raw/master/02_常用标签及属性/banner.png)

## ol li（有序列表）

> li 前面是数字

    <ol>
        <li>item1</li>
        <li>item2</li>
        <li>item3</li>
        <li>item4</li>
    </ol>

* 也可以用来做导航

## dl dt dd（定义列表）

> 可以自定义列表

    <dl>
        <dt>自定义列表标题</dt>
        <dd>dl-item1</dd>
        <dd>dl-item2</dd>
        <dd>dl-item3</dd>
        <dd>dl-item4</dd>
    </dl>

## strong（强调 - 加粗 - 利于SEO）

> 加粗字体，使用 strong 可以利于SEO优化

    <strong>强调</strong>

## em（强调 - 倾斜 - 利于SEO）

    <em>倾斜</em>

## sub（下标）

    <sub>下标</sub>

## sup（上标）

    <sup>上标</sup>

## br（换行）

    <br />

## i（斜体）

    <i>倾斜</i>

## hr（定义水平线）

    <hr />

* hr 基本没啥用，因为一条横线用很多的标签都可以做成一条横线

## 外边距合并

> 父级标签定义了 margin-top，子标签也定义了 margin-top 就会与父级 margin-top合并（**保留较大的那个 margin-top 值**）。**注：只有垂直方向上才会发生外边距合并。**

解决方案：

1. 为父级盒子的顶部加边框

2. 为父级盒子加 padding-top 来隔开两个盒子（**常用**）

* 问：给父级盒子加 padding-top 后，我的盒子就变高了呀，我想让它的大小不变，怎么办？

* 答：给高度减去多的那部分 padding 值。

练习：

完成如下图片展示效果：

![image](https://github.com/MrQuJL/html-quick-start/raw/master/02_常用标签及属性/example.png)

代码如下：

    ```
    <!doctype html>
    <html>
    <head>
        <meta http-equiv='Content-Type' content='text/html;charset=utf-8' />
        <title>图片展示效果</title>
        <meta name='keywords' content='关键词,关键词' />
        <meta name='description' content='网站描述' />
        <style type="text/css">
            *{margin:0;padding:0;}
            body{background-color:#eee;font-size:14px;}
            li{list-style:none;}
            div{
                width:280px;
                height:380px;
                border:20px solid #fff;
                margin:50px auto;
                background-color:#fff;
            }
            div ul li a{
                color:black;
                text-decoration:none;
            }
            div ul{
                padding-top:6px;
            }
            div ul li{
                padding-bottom:10px;
            }
        </style>
    </head>
    <body>
        <div>
            <img src="images/1.png" alt="香奈儿" />
            <ul>
                <li>
                    <a href="#" title="水之密语靓彩">【shaiya莹】水之密语靓彩</a>
                </li>
                <li>
                    <a href="#" title="千金净雅妇科专用">【抢新品NO.120】千金净雅妇科专用</a>
                </li>
                <li>
                    <a href="#" title="千金净雅妇科专用">【抢新品NO.120】千金净雅妇科专用</a>
                </li>
            </ul>
        </div>
    </body>
    </html>
    ```
