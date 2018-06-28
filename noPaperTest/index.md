# index
##### 定义：

	全局公用的classes集合以及包含CSS reset，包含了如下：
	
		1. 布局
		2. 字体
		3. 内外边距  		//antd组件
		4. 按钮 				//antd组件
		5. 输入框			//antd组件
		6. 修改antd框架UI
	
	整站几乎都用到classes集合的class，影响着整站的UI布局，请谨慎更改该文档

**布局**
	
	#root //布局最外层盒子宽度

<div id="root">布局最外层盒子宽度</div>

	

	float:
		- float_l //左浮动

<div id="root">
	<p class="float_l pad-base defaults-bg mar-base">左浮动</p>
	左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动左浮动
</div>

    - float_r //右浮动
		 
<div class="wrap">
	<p class="float_r pad-base defaults-bg mar-base">右浮动</p>
	右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动右浮动
</div>

	- f-clear //清楚浮动
		 
<div class="wrap f-clear">
	<p class="float_r pad-base defaults-bg mar-base">右浮动</p>
	清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动清楚浮动
</div>

	display: 
		
	- display_inb //行内块元素
		 
<div id="root">
	<p class="display_inb">行内块元素</p>
	<p class="display_inb">行内块元素</p>
</div>

	- display_b //此元素将显示为块级元素
		 
<div id="root">
	<span class="display_b">
	此元素将显示为块级元素，此元素前后会带有换行符此元素将显示为块级元素，此元素前后会带有换行符此元素将显示为块级元素，此元素前后会带有换行符此元素将显示为块级元素，此元素前后会带有换行符
	</span>
</div>

	- display_n //此元素不会被显示
		 
<div id="root">
	<p class="display_n">
	此元素不会被显示
	</p>
</div>

**字体**

	h1,.h1 - h6,.h6 //特殊字体大小

<div id="root">
	<span class="h1">h1</span>
	<span class="h2">h2</span>
	<span class="h3">h3</span>
	<span class="h4">h4</span>
	<span class="h5">h5</span>
	<span class="h6">h6</span>
</div>

	text-algin:
		- text_l //左对齐

<div id="root">
	<p class="text_l">左对齐</p>
</div>

	- text_r //右对齐
		 
<div id="root">
	<p class="text_r">右对齐</p>
</div>

	- text_c //居中
				 
<div id="root">
	<p class="text_c">居中</p>
</div>

	color:
	- text_tips 

<div id="root">
	<p class="text_tips">text_tips</p>
</div>

	- text_primary

<div id="root">
	<p class="text_primary">text_primary</p>
</div>

	- text_wrong 

<div id="root">
	<p class="text_wrong">text_wrong</p>
</div>

	- text_promp 
		
<div id="root">
	<p class="text_prompg">text_promp</p>
</div>
		
##### 重置作用:

	无需编写重复代码，便于维护，直接使用需要的class方可
