# margin负值

* margin 除了可以设置正值外，还可以设置负值。

![image](https://github.com/MrQuJL/html-quick-start/raw/master/06_margin负值/images/margin负值.png)

代码如下：

    <!doctype html>
    <html>
    <head>
        <meta http-equiv='Content-Type' content='text/html;charset=utf-8' />
        <title>margin负值</title>
        <meta name='keywords' content='关键词,关键词' />
        <meta name='description' content='网站描述' />
        <style type="text/css">
            *{margin:0;padding:0;}
            .box{
                width:400px;
                height:400px;
                border:1px solid red;
                margin:50px auto;
            }
            .box .mini{
                width:100px;
                height:100px;
                background:green;
                margin:0px 0px 0px 0px;
            }
            
        </style>
    </head>
    <body>
        <div class="box">
            <div class="mini"></div>
        </div>
    </body>
    </html>

**可以以此来理解一下 background-positon 设置负值的情况。**
