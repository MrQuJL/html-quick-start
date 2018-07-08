# form 表单元素

## form

* ```<form action='xxx.action' method='post'></form>```

* action：表单提交的 url 地址，是一个 servlet 还是一个 jsp 页面

* method：发送 form 中数据的 http 方法

* target：规定 action 属性中提交的页面再何处打开

* form 元素是块级元素，其前后会换行

## form 中的控件

input 中的 type 类型

* text：文本框
* password：密码
* radio：单选按钮，要指定相同的name
* checkbox：复选框
* label 标签为 input 元素定义标注
* checked：属性定义默认选中的 input 元素
* disabled：属性规定应该禁用的 input 元素
* submit：提交 form 中的数据
* reset：重置表单中的数据
* button：按钮，多数情况下，用于通过 JavaScript 启动脚本
* image：图片（有提交功能，一般不用，一般给image标签加超链接的方式来模拟）
* hidden：隐藏域（一般在修改页面隐藏用户的id，提交表单时一并同表单数据发送给服务器）




