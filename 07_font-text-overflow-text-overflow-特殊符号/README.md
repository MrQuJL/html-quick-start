# font text overflow text-overflow 特殊符号

## font（字体）

### color（字体颜色）

    color:red; /*同样支持16进制写法，rgb以及rgba*/

### font-size（字体大小）

    font-size:12px;

### font-family（字体类型）

    font-family:'Microsoft Yahei'; /*微软雅黑*/
    font-family:'SimSun'; /*宋体*/
    font-family:'sans-serif'; /*手机字体*/
    font-family:'sans-serif','SimSun','Microsoft Yahei'; /*有多个值的时候优先使用前面的，前面的没有使用后面的*/

### font-weight（字体加粗）

    font-weight:normal; /*字体正常显示*/
    font-weight:bold; /*字体加粗*/
    font-weight:100; /*比较细 100~900之间*/
    font-weight:400; /*默认粗细*/
    font-weight:600; /*加粗==bold*/
    /*100~399是一样的效果*/
    /*400~599是一样的效果*/
    /*600~900是一样的效果*/

### font-style（字体样式）

    font-style:normal; /*正常*/
    font-style:italic; /*斜体-意大利比萨斜塔（斜度大）*/
    font-style:oblique; /*倾斜（斜度小，不明显）*/

### font-variant（规定小型的大写字母）

    font-variant:normal; /*正常*/
    font-variant:small-caps; /*定义小型大写字母（字母是大写的，但是字号很小）*/

### line-height（行高）

    line-height:30px;
    height:30px;
    /*tips:把盒子的高度和文字的行高设置成相同的值可以使文字上下居中*/
    line-height:100%; /*文字多大，行高多大，与font-size有关*/
    line-height:1.2em; /*相当于120%*/
    line-height:1.5; /*相当于150%*/

### 复合写法

    font的基本型：
    font:font-size/line-height font-family;
    /*字体大小，行高，字体类型必须有，而且必须按照上面的顺序，如果要加其他的分样式需要加在font-size之前*/
    /*也可以不写行高，但是不能不写font-size和font-family*/
    例：
    font:small-caps italic bold 50px 'SimSun';
    /*注：color不能写在复合样式里面*/

## text

### text-transform（转换字母大小写）

    text-transform:uppercase; /*大写*/
    text-transform:lowercase; /*小写*/
    text-transform:capitalize; /*首字母大写*/

### text-align（文本水平对齐方式）

    text-align:center; /*文本居中对齐*/
    text-align:left; /*文本居左对齐*/
    text-align:right; /*文本居右对齐*/
    text-align:justify; /*文本两端对齐，文字占满一行的情况下才可以两端对齐*/

### text-indent（文本缩进）

    text-indent:20px; /*首行缩进20像素*/
    text-indent:2em; /*首行缩进两个汉字*/

### text-decoration（文本修饰）

    text-decoration:underline; /*下划线*/
    text-decoration:line-through; /*删除线*/
    text-decoration:overline; /*上划线*/
    text-decoration:none; /*不要修饰*/

### letter-spacing（字符间距）

    letter-spacing:10px; /*每个字符间10px的间距*/

### word-spacing（单词/字间距）

    word-spacing:10px; /*根据文本之间是否有空格来判断是不是一个单词*/

### white-space（换行方式）

    white-space:normal; /*默认不换行*/
    white-space:nowrap; /*文本不会换行，文本会在同一行上继续显示（即使超出了盒子的宽度），直到遇到<br> 标签为止*/

### word-break（拆分单词进行换行）

    word-break:break-all; /*如果是单词需要占两行的话会对单词进行拆分然后再换行*/

## overflow（内容溢出）

    overflow:hidden;（里面的内容超出的时候隐藏）

## text-overflow（css3 规定当文本溢出时的处理方式）

    white-space:nowrap;
    line-clamp:2;
    overflow:hidden;
    text-overflow:elipsis;
    /*被修剪的文本用...符号来代表（只能省略一行）*/

    div p{
        width:100px;s
        border:1px solid red;
        display:-webkit-box;
        -webkit-line-clamp: 3; /*第3行省略...*/
        word-wrap:break-word;
        word-break:break-all;
        overflow:hidden;
        text-overflow:ellipsis;
        -webkit-box-orient:vertical;
    }
    /*文本多行换行省略*/

## 特殊符号

    &nbsp; 空格符
    &lt; 小于符号
    &gt; 大于符号
    &copy; 版权
    &reg; 注册商标





