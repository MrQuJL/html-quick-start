# 高级选择器 属性选择器 a伪类 伪元素选择器

## 高级选择器

### 多元素选择器

	div, p{margin:0;padding:0;}
	/*div和p标签*/

### 后代选择器

	div p{width:100px;height:100px;}
	/*div里面的所有p标签*/

### 子元素选择器

	div > p{color:red;}
	/*匹配div里的直接子p标签*/
	
	<div>
		<h1><p>孙子p</p></h1>
		<p>直接子p</p> <!-- 该p会被选中 -->
	</div>
	
### 毗邻元素选择器

	div + p{color:red;}
	/*匹配与div同级的下面的紧邻的那个p标签*/

	<p>p上</p>
	<div></div>
	<p>p下</p> <!--该p标签中的字体颜色会变红-->
	<p>p下下</p>

## 属性选择器

### [attr]

	[class]{background:red;}
	[id]{background:green;}
	[title]{color:#fff;}
	/*匹配所有具有attr属性的元素*/
	<div id='' class='' title=''></div>

### [attr=val]

	[class='box']{background:red;}
	/*匹配所有具有class属性并且其值等于'box'的元素*/
	<div class='box'></div>

### [attr~=val]
	
	[class~='box']{background:red;}
	/*匹配所有具有att属性并且其值包含'box'或者等于'box'的元素(box必须是一个完整词)
*/
	<div class="box x">div1</div> <!-- 匹配 -->
	<div class="box">div2</div> <!-- 匹配 -->
	<div class="box1"></div> <!-- 不匹配 -->

### [attr|=val]
	
	[class|='box']{background:red;}
	/*匹配所有具有att属性并且其值以'box-'开头或等于'box'的元素（比如说zh-cn），可以有多个值*/
	<div class="box">div</div> <!-- 匹配 -->
	<div class="box-1">div</div> <!-- 匹配 -->
	<div class="boxx-1">div</div> <!-- 不匹配 -->
	<div class="box box-3">div</div> <!-- 不匹配 -->
	<div class="box-3 box">div</div> <!-- 匹配 -->

### [attr1][attr2=val]

	[class][id]{background:red;}
	/*组合属性选择器*/
	<div class="box">div</div> <!-- 不匹配 -->
	<div class="box" id="div2">div</div> <!-- 匹配 -->

	p[class][id]{color:red;}
	/*匹配是p标签并且具有class属性和id属性的元素*/









