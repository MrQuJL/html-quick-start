# 样式初始化-标签的三大类型-text-align

## 样式初始化

    body,dl,dd,p,h1,h2,h3,h4,h5,h6{margin:0;}
    ol,ul{margin:0;padding:0;list-style:none;} /*去除li的小黑原点*/
    a{text-decoration:none;}
    img{border:none;} /*兼容IE6及以下版本*/

* **css reset 原则：但凡是浏览器默认的样式都不要使用。**

* 注：如果对页面加载速度没有太大的要求，可以简写为如下的格式：

    *{margin:0;padding:0;}

* 注：为 img 标签加 ```display:block``` 样式可以去除图片标签下方的空白。

## 标签的三大类型

### 块级标签（block）

    div, p, dl, dt, dd, h3, ul, ol...

块级标签的特征：

1. 默认宽度 100%

2. 支持**手动设置**宽度和高度

3. 独占一行

4. 支持所有的 CSS 样式

### 内联标签（inline）

    span, a, strong, em, i, b...

内联标签特征：

1. 默认宽度由内容撑开

2. 可以和同类标签在一行内展示（友好）

3. **不可以手动设置宽高**

4. 不支持上下 margin，只支持左右 margin，**margin:auto失效**

5. 支持所有 padding，但是上下padding会盖住原有元素（危险），左右 padding 没事

6. span 与 span 之间的空格和回车会被解析

### 行内块级标签（inline-block）

行内块级标签特征：既支持块级标签的属性又支持块级标签的属性

1. 默认内容撑开宽度

2. 支持宽高

3. 可以一排显示（友好）

4. 支持所有 margin，padding，但是不支持 margin:auto

5. 标签与标签之间的空格或回车会被解析

6. IE6,7 不支持块级标签的 inline-block

## 其他

* 使用 display:none 来隐藏一个标签。

* img **可以通过给父级加 text-align 来控制图片的位置**，支持宽高可以一行显示，使用 display:block 来消除底部空白。

### text-align（文本水平对齐方式）

* center：居中对齐，还可以让内部的 inline 和 inline-block 居中，弥补了 inline 和 inline-block 不能居中的不足。

* left：左对齐

* right：右对齐

## FAQ

* 问题1：如何让 span 具备块级标签的特性？

* 答：为 span 标签添加 css 样式：display:block。

* 问题2：如何让 div 具备内联标签的特性？

* 答：为 div 标签添加 css 样式：display:inline。

## 练习：

完成如下图片展示效果：

![image](https://github.com/MrQuJL/html-quick-start/raw/master/04_样式初始化-标签的三大类型-text-align/products.png)

代码如下：

    <!doctype html>
    <html>
    <head>
        <meta http-equiv='Content-Type' content='text/html;charset=utf-8' />
        <title>商品横排展示练习</title>
        <meta name='keywords' content='关键词,关键词' />
        <meta name='description' content='网站描述' />
        <style type="text/css">
            *{margin:0;padding:0;}
            body{background-color:#f5f5f5;}
            div.container{
                width:1170px;
                height:228px;
                margin:100px auto;
            }
            div.container div.item{
                width:210px;
                height:208px;
                background:#fff;
                padding:20px 0 0 20px;
                display:inline-block; /*一行内排列，每一项之间有间隔是因为标签之间的空格或回车会被解析*/
            }
            div.container div.item div.info p.title a{
                text-decoration:none;
                font-size:18px;
                color:#000;
            }
            div.container div.item div.info p.sub-title{
                font-size:14px;
                color:#64C333;
            }
            div.container div.item div.img{
                text-align:right;
            }
        </style>
    </head>
    <body>
        <div class="container">
            <div class="item">
                <div class="info">
                    <p class="title">
                        <a href="#">大家电年度盛典</a>
                    </p>
                    <p class="sub-title">疯抢300元优惠券</p>
                </div>
                <div class="img">
                    <img src="imgs/1.jpg" alt="大家电年度盛典" width="154px" height="154px" />
                </div>
            </div>
            <div class="item">
                <div class="info">
                    <p class="title">
                        <a href="#">冬季孕妇毛衣专场</a>
                    </p>
                    <p class="sub-title">时尚潮流温暖舒适</p>
                </div>
                <div class="img">
                    <img src="imgs/2.jpg" alt="冬季孕妇毛衣专场" width="154px" height="154px" />
                </div>
            </div>
            <div class="item">
                <div class="info">
                    <p class="title">
                        <a href="#">乔丹童鞋跑鞋</a>
                    </p>
                    <p class="sub-title">释放双脚跑起来</p>
                </div>
                <div class="img">
                    <img src="imgs/3.jpg" alt="乔丹童鞋跑鞋" width="154px" height="154px" />
                </div>
            </div>
            <div class="item">
                <div class="info">
                    <p class="title">
                        <a href="#">双12整车特卖啦</a>
                    </p>
                    <p class="sub-title">贷款买车24期0利率</p>
                </div>
                <div class="img">
                    <img src="imgs/4.jpg" alt="双12整车特卖啦" width="154px" height="154px" />
                </div>
            </div>
            <div class="item">
                <div class="info">
                    <p class="title">
                        <a href="#">品牌岁末疯抢</a>
                    </p>
                    <p class="sub-title">分期免息</p>
                </div>
                <div class="img">
                    <img src="imgs/5.jpg" alt="品牌岁末疯抢" width="154px" height="154px" />
                </div>
            </div>
        </div>

    </body>
    </html>

