1. html简介，h5，css3关系

2. html模板配置

3. 各头标签简介，单双标签举例，闭合方式
	双：div
	单：img
盒子模型-双标签里面可以放内容-单标签不可以写内容

4. 开发者工具F12的使用

	1)鼠标滑到某个标签上的时候：标签的颜色意义（蓝色，肉色），标签名，盒子的宽，高

	2)右侧的一些样式信息，直观的看盒子模型


6. css

	1)style标签（type=text/css）

	2)行内样式，内部样式，外部样式

	3)写法：/*宽度:100像素*/

	4)css里面的注释方法

	5)对比html注释

	6)分号结尾

	7)width,height,background

	8)选择器{样式}

7. js

	1)script标签<script type="text/javascript"></script>

	2)简单用法


8. editplus

	1)快捷颜色选择


9. border
	
	1)多边框复合样式：
		border:1px solid red; /*边框大小 边框类型 边框颜色*/
	
	3)多边框单样式:
		border-width:1px;
		border-style:solid;
		border-color:black;
	
	4)单边框复合样式
		border-top:10px solid green;
		border-right:15px solid green;
		border-bottom:10px solid green;
		border-left:10px solid green;

	5)单边框单样式：
		border-top-width:10px;
		border-top-style:solid;
		border-top-color:yellow;

	边框类型：
		solid -- 实线
		dashed -- 虚线
		dotted -- 点线
		double -- 双横线

10. padding(处于boder和实际内容之间)
	
	1)内边距：边框以内，内容以外
		padding:10px;
	
	2)四个值：
		
		padding:5px 10px 15px 20px; /*上 右 下 左（顺时针）*/
		
		padding:5px 10px 15px; /*上 左右 下*/
		
		padding:5px 10px; /*上下 左右*/
		
		padding:5px; /*上下左右*/

	3)一个方向的padding

		padding-top:10px;

		padding-right:10px;

		padding-bottom:10px;

		padding-left:10px;

11. margin

	1)（外边距）边框与外面元素的距离
		margin:10px;
	
	2)四个值：
		
		margin:5px 10px 15px 20px; /*上 右 下 左（顺时针）*/
		
		margin:5px 10px 15px; /*上 左右 下*/
		
		margin:5px 10px; /*上下 左右*/
		
		margin:5px; /*上下左右*/

	3)一个方向的margin

		margin-top:10px;

		margin-right:10px; /*距离右边如果很远则以较远的距离为准*/

		margin-bottom:10px; /*距离下边如果很远则以较远的距离为准*/

		margin-left:10px;
	
	

通配符选择器：*{margin:0;padding:0;}
解决body标签默认8px外边距的问题
p标签默认有16px的外边距
body{margin:0;}

其他的标签也有一些默认的外边距，用通配符选择器全部清空

盒子的大小计算 = 内容大小（width height） + 内边距（padding） + 边框（border）;

12. 单位%

	宽高占父标签的百分比

13. color
	一：英文颜色单词
	二：#十六进制颜色值
	三：rgb(0-255,0-255,0-255)
		255表示那个颜色的最大值
	四：rgba(0-255,0-255,0-255,0-1)
		0表示完全透明
		1表示完全不透明
	
练习

写一个 div，要求如下：

border 大小是 5 10 15 20 的盒子（用单样式写）
margin 大小是 20 15 10 5 的盒子（用单样式写）
padding大小是 40 30 20 10的盒子（用单样式写）

