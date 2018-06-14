# font text overflow

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



## overflow



