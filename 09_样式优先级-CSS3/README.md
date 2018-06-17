# 选择器优先级 样式 样式优先级 CSS3

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

    div{background:red !important;} /*优先级最大*/





