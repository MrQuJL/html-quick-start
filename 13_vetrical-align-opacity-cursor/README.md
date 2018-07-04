# vetrical-align img特征 cursor opacity

## vertical-align 垂直对齐方式

定义行内元素的基线相对于该元素所在行的基线的垂直对齐。
inline  inline-block img图片标签才具有

* top			元素的顶端与行中最高元素的顶端对齐

* middle		此元素放置在父元素的中部。

* bottom		元素的顶端与行中最低的元素的顶端对齐。

* text-top		元素的顶端与父元素字体的顶端对齐

* text-bottom	把元素的底端与父元素字体的底端对齐。

* baseline		默认。元素放置在父元素的基线上。

* 加vertical-align的同排元素都要vertical-align；

* vertical-align可以解决img下方间隙问题；

## img特征

* 支持宽高

* 支持margin（横排展示）

* 能设置text-align

* 能设置vertical-align

* 问题：标签中间隙被解析，不支持marginauto;

## cursor（指针样式）

* cursor: pointer | text | move ......

* default: 默认光标（通常是一个箭头）

* auto: 默认，浏览器设置的光标。

* pointer: 光标呈现为指示链接的指针（一只手）

* move: 此光标指示某对象可被移动。

* text: 光标指示文本。

* wait: 光标指示正忙（通常是一只表或沙漏）。

* help: 光标指示帮助（通常是一个问号或一个气球）。

* 自定义指针样式：cursor:url(hand.cur),pointer;

## opacity

* opacity 属性设置元素的不透明级别

* 标准 不透明度：opacity:0~1; 

* 从 0（完全透明）

* 到 1（完全不透明）

* IE 滤镜： filter:alpha(opacity=0~100);

* 从 0（完全透明）

* 到 100（完全不透明）

