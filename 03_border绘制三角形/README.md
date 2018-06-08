# border绘制三角形

## 原理

* 将盒子的宽高设为0，将底部边框设为none，左右边框颜色设为透明（transparent）即可

## 效果

![image](https://github.com/MrQuJL/html-quick-start/raw/master/03_border绘制三角形/triangle.png)

## 代码

	<!doctype html>
	<html>
	<head>
		<meta http-equiv='Content-Type' content='text/html;charset=utf-8' />
		<title>三角形</title>
		<meta name='keywords' content='关键词,关键词' />
		<meta name='description' content='网站描述' />
		<style type="text/css">
			*{margin:0;padding:0;}
			br{width:100px;height:100px;background-color:#fff;} /*无效*/
			div{margin-bottom:10px;}
			.box1{
				width:100px;
				height:100px;
				background:red;
				border-width:100px;
				border-style:solid;
				border-color:green blue pink #660099;
			}
			.box2{
				width:0;
				height:0;
				background:red;
				border-width:100px;
				border-style:solid;
				border-color:green blue pink #660099;
			}
			.box3{
				width:0;
				height:0;
				background:red;
				border-width:100px;
				border-style:solid;
				border-color:green blue pink #660099;
				border-bottom:none;
			}
			.box4{
				width:0;
				height:0;
				border-width:100px;
				border-style:solid;
				border-color:green blue pink #660099;
				border-bottom:none;
				border-left-color:rgba(0,0,0,0);
				border-right-color:rgba(0,0,0,0);
			}
			.box5{
				width:0;
				height:0;
				border-width:100px;
				border-style:solid;
				border-color:green blue pink #660099;
				border-left:none;
				border-top-color:rgba(0,0,0,0);
				border-bottom-color:rgba(0,0,0,0);
			}
			.box6{
				width:0;
				height:0;
				border-width:100px;
				border-style:solid;
				border-color:green blue pink #660099;
				border-right:none;
				border-top-color:rgba(0,0,0,0);
				border-bottom-color:rgba(0,0,0,0);
			}
			.box7{
				width:0;
				height:0;
				border-width:100px;
				border-style:solid;
				border-color:green blue pink #660099;
				border-top:none;
				border-left-color:transparent;
				border-right-color:transparent;
			}
		</style>
	</head>
	<body>
		<div class="box1"></div>
		<div class="box2"></div>
		<div class="box3"></div>
		<div class="box4"></div>
		<div class="box5"></div>
		<div class="box6"></div>
		<div class="box7"></div>
		<br />
	</body>
	</html>



