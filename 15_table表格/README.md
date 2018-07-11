# table

## table表格结构

```<table>标签定义HTML表格```

* table 表格
* thead 表格头
* tbody 表格主体
* tfoot 表格尾
* tr 定义表格行
* th 定义表头 **（居中）**
* td 定义表格单元

## table的默认特征

1. 单元格默认平分table 的宽度
2. th里面的内容默认加粗并且左右上下居中
3. td里面的内容默认上下居中 左对齐显示
4. table 决定了整个表格的宽度；
5. table里面的单元格宽度会被转换成百分比；
6. 表格里面的每一列必须有宽度；
7. 表格同一列/行会继承最大值；
8. th,td中没有margin
9. 单元格可以包含:(文本、图片、列表、段落、表单、表格) 等等。

## table样式重置

* 属性：

* width 规定表格的宽度

* height 规定表格的高度

* border 规定表格边框的宽度

* 样式属性：

* border-spacing:X Y 指定单元格边界之间的水平和垂直间距

* border-collapse:collapse 如果可能，边框会合并为一个单一的边框。会忽略 border-spacing

### 表格样式重置

* table{border-collapse:collapse;} 

* th,td{padding:0;} 重置单元格默认填充








