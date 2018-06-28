# variables

##### 定义：

		整站UI底层变量集合，包含如下：

		1. font
		2. status
		3. radius
		4. Evaluation grade
	
	
	以上所有的模块都由不同的变量集合，影响着整站的UI布局，请谨慎更改该文档

**font**
	
	定义了整站所用的字体，字体颜色，字体大小。 

		字体： base。 
		字体颜色：@fill-base/@fill-tips/@color-text-base
		字体大小：@fontSizeLg/@fontSizeMd/@fontSizeM。

**status**
	
	定义了整站交互状态UI展示：
		@free-color //免费获取
		@no-free-color //购买
		@no-evaluation-color //已购未测
		@evaluation-color //查看测评
		@keep-evaluation-color //继续测评。

**radius**
	
	定义了整站中盒子的圆角：
		@radius-xs //xs
		@radius-sm //sm
		@radius-md //md
		@radius-lg //lg
		@radius-circle //50%

**Evaluation grade**
	
	定义了整站测评等级交互UI展示：
		@fail-color //< 60 差
		@pass-color //<80 && >= 60 及格
		@fine-color //已购未测 >=80 优秀



##### 重置作用:

	便于调用，后期UI全局更改，只需更改setting文档，无需更改所牵涉到的组件或私有UI

##### variables.less

    //字体
    @fontSizeLg:36px;
    
    @fontSizeMd:30px;
    
    @fontSizeM:28px;
    
    @fill-base:#fff;
    
    @fill-tips:#aaa;
    
    @color-text-base:#25272c;
    
    @brand-primary:#4782f6;
    
    @wrong-color:#e22124;
    
    @prompt-color:#ff7304;
    
    @h-spacing-lg: 24px;
    @v-spacing-lg:24px;
    
    //试卷状态
    @free-color: #87d37b;
    @no-free-color: #ff3a31;
    @no-evaluation-color: #4782f6;
    @evaluation-color: #ff7304;
    @keep-evaluation-color: #4782f6;
    
    //测评等级
    @fail-color: #ff3a31;
    @pass-color: #ffcc33;
    @fine-color: #87d37b;
    
    // 圆角
    @radius-xs: 4px;
    @radius-sm: 6px;
    @radius-md: 10px;
    @radius-lg: 20px;
    @radius-circle: 50%;
    
    @base-border-color:#edeff0;
    
    @border-tips-color: #aaa;
    
    @base-disabled: #ccc;