# 选择器优先级 样式 样式优先级 overflow CSS3

## 选择器优先级

* < 标签 < class < id

## 样式

### 行内样式

    <div style="color:red;">文字</div>

### 内联样式

    <style type="text/css">
        *{margin:0;padding:0;}
    </style>

### 外联样式

    <link rel="stylesheet" href="xx.css" type="text/css" />
    /*其实就是把css单独写成一个文件，使用link标签来引入*/
    
### 通过 import 来引入 css 文件（了解）

    <style>
        @import url("style/index.css"); /*放在第一行*/
    </style>

### Link 与 @import 差异

1. 来源与作用：link 属于HTML 标签，除了可以加载CSS外， 还可以加载其他文件，而@import 完全是CSS提供的一种方式，只能加载CSS。

2. 加载顺序不同：link 引用的CSS会在页面被加载的时候同时加载，而@import 引用的CSS会等到页面全部被下载完再被加载， 所以有时候会出现开始没有样式，之后页面闪烁一下出现样式（在网速慢的时候会更明显）。

## 样式优先级

外链样式 < 嵌入样式 < 行间样式

## ! important

    div{background:red !important;} /*优先级最大，尽量不要使用*/

## CSS3

### border-radius（圆角）

    border-radius:10px 10px 10px 10px; /*左上 右上 右下 左下*/
    border-radius:10px 20px 10px; /*左上 右上+左下 右下*/
    border-radius:50px 10px; /*左上+右下 右上+左下*/
    border-radius:50px; /*左上 右下 右上 左下*/
    
    border-top-left-radius:10px; /*左上角*/
    border-top-right-radius:10px; /*右上角*/
    border-bottom-left-radius:10px; /*左下角*/
    border-bottom-right-radius:10px; /*右下角*/

怎么画圆呢？

    border-radius:50%; /*前提盒子是正方形*/
    /*最多只能圆到50%*/

怎么画胶囊呢？（常用于画按钮）

    width:400px;
    height:100px; /*高度矮一点*/
    border-radius:50%;

### box-shadow（盒子阴影）

* h-shadow 水平偏移量，允许负值（必须）

* v-shadow 垂直偏移量，允许负值（必须）

* blur 模糊半径（可选）

* spread 阴影的大小（可选）

* color 阴影的颜色（可选）

* 外部阴影（默认） 内部阴影（inset可选）


    box-shadow:20px 0px 5px 2px #000;
    box-shadow:0px 0px 15px 2px #ddd inset;

## overflow（内容溢出）

* visible（默认，显示）

* hidden（隐藏）

* auto（会根据宽高的溢出情况自动出现滚动条或者不出现滚动条）

* scroll（无论图片有没有超出父级的宽度都会出现滚动条）

## overflow-x（只针对x轴进行操作）

    overflow-x:hidden;

## overflow-y（只针对y轴进行操作）

    overflow-y:hidden;

## opacity（盒子透明）

    opactity: 透明 0~1; /*0 完全透明 1 完全不透明*/
    /*并没有消失*/
    opactity:0.5;
    filter:alpha(opacity=1~100); /*若想兼容IE加上这句*/

    一个颜色值：transparent（透明）
