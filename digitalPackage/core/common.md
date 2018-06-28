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

<div class="wrap">布局最外层盒子宽度</div>

	float:
		- float-l //左浮动

<div class="wrap">
	<p class="float-l pad-base defaults-bg mar-base">左浮动</p>
	左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动
</div>

    - float-r //右浮动
		 
<div class="wrap">
	<p class="float-r pad-base defaults-bg mar-base">右浮动</p>
	右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动
</div>

	- f-clear //清楚浮动
		 
<div class="wrap f-clear">
	<p class="float-r pad-base defaults-bg mar-base">右浮动</p>
	清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动
</div>

	display: 
		- display-in //此元素会被显示为内联元素，元素前后没有换行符

<div class="wrap">
	<p class="display-in">此元素会被显示为内联元素，元素前后没有换行符</p>
	<p class="display-in">此元素会被显示为内联元素，元素前后没有换行符</p>
</div>

	- display-inb //行内块元素
		 
<div class="wrap">
	<p class="display-inb">行内块元素</p>
	<p class="display-inb">行内块元素</p>
</div>

	- display-b //此元素将显示为块级元素
		 
<div class="wrap">
	<span class="display-b">
	此元素将显示为块级元素，此元素前后会带有换行符此元素将显示为块级元素，此元素前后会带有换行符此元素将显示为块级元素，此元素前后会带有换行符此元素将显示为块级元素，此元素前后会带有换行符
	</span>
</div>

	- display-none //此元素不会被显示
		 
<div class="wrap">
	<p class="display-none">
	此元素不会被显示
	</p>
</div>

**字体**
	
	ellipsis //省略号

<div class="wrap">
	<p class="ellipsis" style="width:100px;height:48px">省略号省略号省略号省略号省略号</p>
</div>

	h1,.h1 - h6,.h6 //特殊字体大小

<div class="wrap">
	<span class="h1">h1</span>
	<span class="h2">h2</span>
	<span class="h3">h3</span>
	<span class="h4">h4</span>
	<span class="h5">h5</span>
	<span class="h6">h6</span>
</div>

	text-algin:
		- text-l //左对齐

<div class="wrap">
	<p class="text-l">左对齐</p>
</div>

		- text-r //右对齐
		 
<div class="wrap">
	<p class="text-r">右对齐</p>
</div>

		- text-c //居中
				 
<div class="wrap">
	<p class="text-c">居中</p>
</div>

	color:
		- font-primary //突出文字

<div class="wrap">
	<p class="font-primary">突出文字</p>
</div>

		- font-weak //辅助色

<div class="wrap">
	<p class="font-weak">辅助色</p>
</div>

		- font-danger //错误用色

<div class="wrap">
	<p class="font-danger">错误用色</p>
</div>

		- font-warning //醒目、提醒用色，例如购买
		
<div class="wrap">
	<p class="font-warning">醒目、提醒用色，例如购买</p>
</div>

		- font-success //正确用色
		
<div class="wrap">
	<p class="font-success">正确用色</p>
</div>

**内外边距**	

	margin： //外边距左右上下

	为了使marign效果淋漓尽致的展示效果，新增class “defaults-bg” 数字包出版项目没有使用这个class
> 


	- mar-base

<div class="mar-base defaults-bg">mar-base</div>

	- mar-md
		
<div class="mar-md defaults-bg">mar-md</div>

	- mar-lg
		
<div class="mar-lg defaults-bg">mar-lg</div>


	- mar-lgd
		

<div class="mar-lgd defaults-bg">mar-lgd</div>


	- mar-sm
		
<div class="mar-sm defaults-bg">mar-sm</div>


	- mar-smd
		
<div class="mar-smd defaults-bg">mar-smd</div>
		
	mar-l： //左外边距
> 


	- mar-l-base
		
<div class="mar-l-base defaults-bg">mar-l-base</div>

	- mar-l-m
		
<div class="mar-l-m defaults-bg">mar-l-m</div>

	- mar-l-md

<div class="mar-l-md defaults-bg">mar-l-md</div>


	- mar-l-lg

<div class="mar-l-lg defaults-bg">mar-l-lg</div>

	- mar-l-lgd

<div class="mar-l-lgd defaults-bg">mar-l-lgd</div>


	- mar-l-sm

<div class="mar-l-sm defaults-bg">mar-l-sm</div>


	- mar-l-smd

<div class="mar-l-smd defaults-bg">mar-l-smd</div>


	mar-r：//右外边距
> 


	- mar-r-base
		
<div class="mar-r-base defaults-bg">mar-r-base</div>

	- mar-r-m
		
<div class="mar-r-m defaults-bg">mar-r-m</div>

	- mar-r-md

<div class="mar-r-md defaults-bg">mar-r-md</div>


	- mar-r-lg

<div class="mar-r-lg defaults-bg">mar-r-lg</div>

	- mar-r-lgd

<div class="mar-r-lgd defaults-bg">mar-r-lgd</div>


	- mar-r-sm

<div class="mar-r-sm defaults-bg">mar-r-sm</div>


	- mar-r-smd

<div class="mar-r-smd defaults-bg">mar-r-smd</div>

	mar-t： //上外边距
> 


	- mar-t-base
		
<div class="mar-t-base defaults-bg">mar-t-base</div>

	- mar-t-m
		
<div class="mar-t-m defaults-bg">mar-t-m</div>

	- mar-r-md

<div class="mar-t-md defaults-bg">mar-t-md</div>


	- mar-t-lg

<div class="mar-t-lg defaults-bg">mar-t-lg</div>

	- mar-t-lgd

<div class="mar-t-lgd defaults-bg">mar-t-lgd</div>


	- mar-t-sm

<div class="mar-t-sm defaults-bg">mar-t-sm</div>


	- mar-t-smd

<div class="mar-t-smd defaults-bg">mar-t-smd</div>
	mar-b：//下外边距
> 


	- mar-b-base
		
<div class="mar-b-base defaults-bg">mar-b-base</div>

	- mar-b-m
		
<div class="mar-b-m defaults-bg">mar-b-m</div>

	- mar-b-md

<div class="mar-b-md defaults-bg">mar-b-md</div>


	- mar-b-lg

<div class="mar-b-lg defaults-bg">mar-b-lg</div>

	- mar-b-lgd

<div class="mar-b-lgd defaults-bg">mar-b-lgd</div>


	- mar-b-sm

<div class="mar-r-sm defaults-bg">mar-b-sm</div>


	- mar-b-smd

<div class="mar-b-smd defaults-bg">mar-b-smd</div>
		
	padding： //内边距左右上下
		
	为了使marign效果淋漓尽致的展示效果，新增class “defaults-bg” 数字包出版项目没有使用这个class
> 


	- pad-base

<div class="pad-base defaults-bg">pad-base</div>

	- pad-md
		
<div class="pad-md defaults-bg">pad-md</div>

	- pad-lg
		
<div class="pad-lg defaults-bg">pad-lg</div>


	- pad-lgd
		

<div class="pad-lgd defaults-bg">pad-lgd</div>


	- pad-sm
		
<div class="pad-sm defaults-bg">pad-sm</div>


	- pad-smd
		
<div class="pad-smd defaults-bg">pad-smd</div>
		
	pad-l： //左内边距
> 


	- pad-l-base
		
<div class="pad-l-base defaults-bg">pad-l-base</div>

	- pad-l-m
		
<div class="pad-l-m defaults-bg">pad-l-m</div>

	- pad-l-md

<div class="pad-l-md defaults-bg">pad-l-md</div>


	- pad-l-lg

<div class="pad-l-lg defaults-bg">pad-l-lg</div>

	- pad-l-lgd

<div class="pad-l-lgd defaults-bg">pad-l-lgd</div>


	- pad-l-sm

<div class="pad-l-sm defaults-bg">pad-l-sm</div>


	- pad-l-smd

<div class="pad-l-smd defaults-bg">pad-l-smd</div>


	pad-r：//右内边距
> 


	- pad-r-base
		
<div class="pad-r-base defaults-bg">pad-r-base</div>

	- pad-r-m
		
<div class="pad-r-m defaults-bg">pad-r-m</div>

	- pad-r-md

<div class="pad-r-md defaults-bg">pad-r-md</div>


	- pad-r-lg

<div class="pad-r-lg defaults-bg">pad-r-lg</div>

	- pad-r-lgd

<div class="pad-r-lgd defaults-bg">pad-r-lgd</div>


	- pad-r-sm

<div class="pad-r-sm defaults-bg">pad-r-sm</div>


	- pad-r-smd

<div class="pad-r-smd defaults-bg">pad-r-smd</div>

	pad-t： //上内边距
> 


	- pad-t-base
		
<div class="pad-t-base defaults-bg">pad-t-base</div>

	- pad-t-m
		
<div class="pad-t-m defaults-bg">pad-t-m</div>

	- pad-r-md

<div class="pad-t-md defaults-bg">pad-t-md</div>


	- pad-t-lg

<div class="pad-t-lg defaults-bg">pad-t-lg</div>

	- pad-t-lgd

<div class="pad-t-lgd defaults-bg">pad-t-lgd</div>


	- pad-t-sm

<div class="pad-t-sm defaults-bg">pad-t-sm</div>


	- pad-t-smd

<div class="pad-t-smd defaults-bg">pad-t-smd</div>
	
	pad-b：//下内边距
> 


	- pad-b-base
		
<div class="pad-b-base defaults-bg">pad-b-base</div>

	- pad-b-m
		
<div class="pad-b-m defaults-bg">pad-b-m</div>

	- pad-b-md

<div class="pad-b-md defaults-bg">pad-b-md</div>


	- pad-b-lg

<div class="pad-b-lg defaults-bg">pad-b-lg</div>

	- pad-b-lgd

<div class="pad-b-lgd defaults-bg">pad-b-lgd</div>


	- pad-b-sm

<div class="pad-r-sm defaults-bg">pad-b-sm</div>


	- pad-b-smd

<div class="pad-b-smd defaults-bg">pad-b-smd</div>



**按钮**
	
	u-btn //默认按钮UI

<div class="u-btn">默认</div>

	u-btn-primary //主色
<div class="u-btn u-btn-primary">主色</div>

	u-btn-warin //警告醒目

<div class="u-btn u-btn-primary">警告</div>

	u-btn-danger //危险

<div class="u-btn u-btn-danger">危险</div>


	u-btn-success //成功


<div class="u-btn u-btn-success">成功</div>


	u-btn-lint //目前用于购买按钮


<div class="u-btn u-btn-lint">购买</div>


	u-btn-disable //禁用


<div class="u-btn u-btn-disable">禁用</div>

	u-btn-sm //按钮xs


<div class="u-btn u-btn-sm">xs</div>


	u-btn-smd //按钮s


<div class="u-btn u-btn-smd">s</div>


	u-btn-m //按钮m


<div class="u-btn u-btn-m">m</div>


	u-btn-md //按钮m+


<div class="u-btn u-btn-md">m+</div>


	u-btn-lg // 按钮l


<div class="u-btn u-btn-lg">l</div>


	u-btn-lgd //按钮l+


<div class="u-btn u-btn-lgd">l+</div>




**输入框**

	u-input //输入框

<div class="wrap">
	<input class="u-inout" placeholder="请输入关键字" />
</div>

	u-input-search //搜索框

<div class="wrap">
	<input class="u-inout u-input-search" placeholder="请输入关键字" />
</div>

**修改layer中弹框UI**
	
	根据UI效果图，更改layer中弹框，满足UI效果
		
##### 重置作用:

	无需编写重复代码，便于维护，直接使用需要的class方可
