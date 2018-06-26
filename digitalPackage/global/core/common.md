# common
##### 定义：

	全局公用的classes集合，包含了如下：
	
		1. 布局
		2. 字体
		3. 内外边距
		4. 按钮
		5. 输入框
		6. 修改layer中弹框UI
	
	整站几乎都用到classes集合的class，影响着整站的UI布局，请谨慎更改该文档

**布局**
	
	wrap //布局最外层盒子宽度
	float：
		- float-l //左浮动
		- float-r //右浮动
		- f-clear //清楚浮动
	display：
		
		- display-in //此元素会被显示为内联元素，元素前后没有换行符
		- display-inb //行内块元素
		- display-b //	此元素将显示为块级元素，此元素前后会带有换行符
		- display-none //此元素不会被显示

**字体**
	
	ellipsis //省略号
	h1,.h1 - h6,.h6 //特殊字体大小
	text-algin:
		- text-l //左对齐
		- text-r //右对齐
		- text-c //居中
	color:
		- font-primary //突出文字
		- font-weak //辅助色
		- font-danger //错误用色
		- font-warning //醒目、提醒用色，例如购买
		- font-success //正确用色

**内外边距**	

	margin： //外边距左右上下
		- mar-base
		- mar-md
		- mar-lg
		- mar-lgd
		- mar-sm
		- mar-smd
		
	mar-l： //左外边距
		-  mar-l-base
		-  mar-l-m
		-  mar-l-md
		-  mar-l-lg
		-  mar-l-lgd
		-  mar-l-sm
		-  mar-l-smd

	mar-r：//右外边距
		- mar-r-base
		- mar-r-m
		- mar-r-md
		- mar-r-lg
		- mar-r-lgd
		- mar-r-sm
		- mar-r-smd

	mar-t： //上外边距
		-  mar-t-base
		-  mar-t-m
		-  mar-t-md
		-  mar-t-lg
		-  mar-t-lgd
		-  mar-t-sm
		-  mar-t-smd

	mar-b：//下外边距
		- mar-b-base
		- mar-b-m
		- mar-b-md
		- mar-b-lg
		- mar-b-lgd
		- mar-b-sm
		- mar-b-smd
		
	padding： //内边距左右上下
		- pad-base
		- pad-md
		- pad-lg
		- pad-lgd
		- pad-sm
		- pad-smd
		
	pad-l： //左内边距
		-  pad-l-base
		-  pad-l-m
		-  pad-l-md
		-  pad-l-lg
		-  pad-l-lgd
		-  pad-l-sm
		-  pad-l-smd

	pad-r：//右内边距
		- pad-r-base
		- pad-r-m
		- pad-r-md
		- pad-r-lg
		- pad-r-lgd
		- pad-r-sm
		- pad-r-smd

	pad-t： //上内边距
		-  pad-t-base
		-  pad-t-m
		-  pad-t-md
		-  pad-t-lg
		-  pad-t-lgd
		-  pad-t-sm
		-  pad-t-smd

	pad-b：//下内边距
		- pad-b-base
		- pad-b-m
		- pad-b-md
		- pad-b-lg
		- pad-b-lgd
		- pad-b-sm
		- pad-b-smd



**按钮**
	
	u-btn //默认按钮UI
	u-btn-primary //主色
	u-btn-warin //警告醒目
	u-btn-danger //危险
	u-btn-success //成功
	u-btn-lint //目前用于购买按钮
	u-btn-disable //禁用
	u-btn-sm //按钮xs
	u-btn-smd //按钮s
	u-btn-m //按钮m
	u-btn-md //按钮m+
	u-btn-lg // 按钮l
	u-btn-lgd //按钮l+

**输入框**

	u-input //输入框
	u-input-search //搜索框

**修改layer中弹框UI**
	
	根据UI效果图，更改layer中弹框，满足UI效果
		
##### 重置作用:

	无需编写重复代码，便于维护，直接使用需要的class方可

### 列子
	
	<div class="u-btn">nih</div>