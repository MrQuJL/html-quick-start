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

6. ```<!-- html注释 -->```

7. ```/* css注释 */```

8. ul,li/ol,li/dl,dt,dd拥有父子级关系的标签；（用了 ul 必须用 li，ul 里面的其他标签必须在 li 里面）

9. **p, dt, h 标签  里面不能嵌套块属性标签；**

10. **a标签不能嵌套a；**

11. **内联元素不能嵌套块；（a除外）**

12. [更多规范请参考](https://github.com/MrQuJL/html-quick-start/blob/master/05_前端规范-选择器初级-background详解/HTML命名行业规范.txt "更多规范请参考")

## 选择器初级

### class选择器

* 相同的 class 名可以在页面中出现多次。

* 同一个标签可以有多个 class，用空格隔开 class 名字。

	```
    <style type="text/css">
        .c1{width:100px;height:100px;} /*选到class名为c1的标签*/
        .c2{background:red;} /*选到class名为c2的标签*/
    </style>
    <div class="c1 c2"></div>
	```

### id选择器

* 一个 id 名在页面中只能出现一次，如果出现多次，查找的 id 总是页面中第一次出现的。

* 一个标签只能有一个 id（具有唯一性）。

	```
    <style type="text/css">
        #unique{color:red;} /*选到id名为unique的标签*/
    </style>
    <div id="unique"></div>
    <!-- 在当前页面的任何地方都不能在使用 unique 这个 id 名 -->
	```

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

* background-color（背景颜色）

	```
	background-color:red;
	```

* background-image（背景图片--位于背景图片之上）

	```
	background-image:url('imgs/1.jpg');
	```

* background-repeat（是否在图片未能铺满盒子的时候平铺满盒子）

	```
	background-repeat:no-repeat; /*不平铺*/
	background-repeat:repeat-x; /*只在x轴平铺*/
	background-repeat:repeat-y; /*只在y轴平铺*/
	background-repeat:repeat; /*x轴和y轴均平铺（默认）*/
	```

* background-position（背景图片位置）

background-position 有两个位置的值（先X后Y - 虽然颠倒位置后浏览器仍然能识别，但是为了规范尽量按照常理来写）：X Y <br/>

X: left center right <br/>

Y: top center bottom <br/>

	```
	background-position:left bottom; /*左下*/
	background-position:right center; /*右中*/
	background-position:center top; /*中上*/
	background-position:right; /*右中 - 如果只给一个值，第二个值默认center*/
	background-position:top; /*上中 - 如果只给一个值，第二个值默认center*/
	```

X: % <br/>

Y: % <br/>

**注：百分比可以给负值，图片可以往外跑。** <br/>

	```
	background-position:20% 30%; /*处于水平的20%，垂直的30%的位置*/
	background-position:-20% 30%;
	background-position:20%; /*如果只给一个值，另一个值是50%*/
	```

X: px <br/>

Y: px <br/>

	```
	background-position:10px 20px; /*图片距左边10px，距离上面20px*/
	```

**注：px也可以给负值，图片可以往外跑。** <br/>

* background-size（css3-背景图片大小）













