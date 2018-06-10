# 前端规范-选择器初级-background详解

## 前端规范

### HTML 命名规范：

* 必须以英文开头，可以包含（-_数字），不能使用中文

* 必须使用小写字母

* 见名知意

* 命名扩展：如果 product 类下面还有子模块可以这么写：product-model1

### 前端规范：

1. 所有书写均在英文半角状态下的小写；

2. id，class 必须以字母开头；

3. 所有标签必须闭合；

4. html标签用tab键缩进；

5. 属性值必须带引号；

6. <!-- html注释 -->

7. /* css注释 */

8. ul,li/ol,li/dl,dt,dd拥有父子级关系的标签；（用了 ul 必须用 li，ul 里面的其他标签必须在 li 里面）

9. **p, dt, h 标签  里面不能嵌套块属性标签；**

10. **a标签不能嵌套a；**

11. **内联元素不能嵌套块；（a除外）**

12. [更多规范请参考](https://github.com/MrQuJL/html-quick-start/blob/master/05_前端规范-选择器初级-background详解/HTML命名行业规范.txt "更多规范请参考")

## 选择器初级

### class选择器

* 相同的 class 名可以在页面中出现多次。

* 同一个标签可以有多个 class，用空格隔开 class 名字。

	<style type="text/css">
		.c1{width:100px;height:100px;} /*选到class名为c1的标签*/
		.c2{background:red;} /*选到class名为c2的标签*/
	</style>
	<div class="c1 c2"></div>

### id选择器

* 一个 id 名在页面中只能出现一次，如果出现多次，查找的 id 总是页面中第一次出现的。

* 一个标签只能有一个 id（具有唯一性）。

	<style type="text/css">
		#unique{color:red;} /*选到id名为unique的标签*/
	</style>
	<div id="unique"></div>
	<!-- 在当前页面的任何地方都不能在使用 unique 这个 id 名 -->

### 标签选择器

	<style type="text/css">
		div{background-color:yellow;} /*选到div标签*/
	</style>
	<div></div>

### 通配符选择器

	<style type="text/css">
		*{margin:0;padding:0;} /*选到所有的标签*/
	</style>

## background详解





