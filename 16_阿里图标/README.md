# 阿里图标 & CSS高级技巧

## CSS高级技巧

CSS继承指的是，特定的CSS属性向下传递到子孙元素

1. 默认继承的有：
	color
	font:small-caps italic bold 50px/100px 'microsoft yahei';
	text-align
	text-indent:
	letter-spacing
	word-spacing
	list-style----只继承ul
	......

2. a 标签的color值不继承

3. 默认不继承的给属性加inherit 例：background:inherit;

4. css重用：一个代码多次利用,通过添加特定的class类来实现

	例如：
	.fL{float:left;}
	.fR{float:right}	
	........

5. 组件化开发：

	网页中不同功能模块，写入不同的css文件

## 阿里图标

### 下载阿里字体图标

	1. 找到阿里图标	
		* 打开百度搜索   ‘ 阿里图标‘
		* 点击进去会进入 阿里图标首页地址：http://www.iconfont.cn/plus
		* 注册一个账号，方便后面的图标统一管理
		* 找到导航栏中的 ---图标库---下方的---官方图标库，这里有很多官方的图标

	2、下载（以天猫图标为例）
		* 在页面中找到 --天猫图标库--
		* 找到需要的图标，鼠标滑入有--添加入库--选项,如此依次操作
		* 都添加好后，在顶部导航栏找到---购物车图标---点击
		* 如果 选中下面的---添加到项目--可以保存起来，方便下次再用，也可以实现与你之前的图标合并，
		* 如果 选中 ---下载---就直接下载了

### 阿里图标使用

1. 我们项目的文件夹新建一个iconfont文件夹，然后将下载好的文件黏贴在里面

2. 使用在项目中使用link标签引入iconfont中的 iconfont.css：
	<link rel="stylesheet" type="text/css" href="./iconfont.css">

3. 在需要使用阿里图标的 class中添加iconfont 类名：
	<i class="iconfont"></i>

4. 点击demo_fontclass.html文档，在浏览器中打开

5. 找到需要的图标，复制下面的icon-xxx名字到<i class="iconfont icon-xxx"></i>作为标签的类型，这样图标就OK了

### ico网站logo

1. 首先得有一个.ico 作为扩展名 文件

2. 通过```<link rel="icon" href="url路径"  type="image/x-icon">```引入即可，具体如下：

	<link rel="shortcut icon" href="/dir/favicon.ico"  type="image/x-icon">













