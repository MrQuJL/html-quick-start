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

	```html
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
	```

* <!doctype html>：html5 的头标记。

* <html></html>：里面放 html 主体。

* <head></head>：html头部，多用于放一些页面加载时需要用到的css，js文件，若页面加载时不需要用到，就不要把css和js放到这里面，会影响页面的打开速度。

* <meta http-equiv='Content-Type' content='text/html;charset=utf-8' />：页面编码utf-8。

* <title>模板</title>：就是显示在浏览器选项卡上的标题。

* <meta name='keywords' content='关键词,关键词' />：用于SEO，当你把网站发布到服务器上的时候，别人搜索一个关键词，就通过这个标记中的信息来查找到你的网页，所以现在有一个行业叫 SEO 优化，专门提升别人网站在百度的搜索排名。

* <meta name='description' content='网站描述' />：就是百度快照中的内容。

* <body></body>：在这里面写 html 代码。

## 单双标签的闭合方式

* 单标签：<img />, <input />

* 双标签：<div></div>, <p></p>

## 开发者工具箱F12的简易用法

打开方式：

	1. 右击 --> 检查
	2. 右击 --> 审查元素
	3. F12

![image](https://github.com/MrQuJL/html-quick-start/raw/master/01_html基础/imgs/box.png)

## css的写法（选择器）

	```html
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
	```

## js的写法

	```javascript
		...
		<body>
		<script type="text/javascript">
			alert(1);
		</script>
		</body>
		...
	```

注：可以放在 body 里面，也可以放在 head 里面。

## border

## padding

## margin

## 盒子大小的计算

## 宽高单位的另一种写法

## 颜色的几种表现形式

## 练习

写一个 div盒子，要求如下：

* border 大小是 5 10 15 20 的盒子（用单样式写）
* margin 大小是 20 15 10 5 的盒子（用单样式写）
* padding大小是 40 30 20 10的盒子（用单样式写）
