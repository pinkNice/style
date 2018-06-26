# setting

##### 定义：

	整个项目所有用到的变量集合，包含了如下：

		1.  color
		2.  space
		3.  margin
		4.  padding
		5.  font
		6.  links
		7.  border
		8.  button
		9.  input
		10. Z-index
	
	
	以上所有的模块都由不同的变量集合，影响着整站的UI布局，请谨慎更改该文档

**color**
	
	定义了整站字体颜色、边框颜色、背景色、链接颜色、鼠标经过颜色、错误颜色提示、警告颜色提示、正确颜色提示

**space**
	
	定义了整站模块之间的间距值，间距值： base/m/md/lg/lgd/sm/smd；便于margin与padding调用。

**margin**	

	定义了整站的模块外边距，外边距： base/m/md/lg/lgd/sm/smd。

**padding**
	
	定义了整站模块内边距，内边距： base/m/md/lg/lgd/sm/smd。

**font**
	
	定义了整站所用的字体，字体颜色，字体大小。 

		字体： base。 
		字体颜色：base/primary/weak/danger/warning/success
		字体大小：base/lg/sm/smaller/lead。
			同时也定义H1-H6字体大小

**links**

	定义了整站链接色，链接色：base/none/darken/underline

**border**
	
	定义了整站边框所有的属性，边框大小、边框颜色、边框圆角。
		边框大小： base
		边框颜色： base/primary/warning/danger/success
		边框圆角： base

**button**

	定义了整站所用的按钮，按钮宽、按钮高、按钮行高、按钮背颜色、按钮字体颜色。
		按钮宽：base-width/m-width/md-width/lg-width/lgd-width/sm-width/smd-width
		按钮高：base-height/m-height/md-height/lg-height/lgd-height/sm-height/smd-height
		按钮颜色：default-bg/primary-bg/waring-bg/danger-bg/success-bg/disable-bg/light-bg/
				primary-ed-bg/waring-ed-bg/danger-ed-bg/success-ed-bg/light-ed-bg
		按钮字体颜色: base

**input**

	定义了整站input相关属性：圆角、边框、内边距。

**Z-index**

	定义了整站元素的堆叠顺序。拥有更高堆叠顺序的元素总是会处于堆叠顺序较低的元素的前面。特别有多个弹框场景时。
	Z-index值：zindex-dropdown/zindex-sticky/zindex-fixed/zindex-modal-backdrop/zindex-modal/
			   zindex-popover/zindex-tooltip
		
##### 重置作用:

	便于调用，后期UI更改，只需更改setting文档，无需更改所牵涉到的组件或私有UI
	
### _setting.scss

	``` ruby
	 @import "mixin";

	// Color system
	$black:       #000 !default;
	$white:       #fff !default;
	$gray:        #aaa !default;
	$gray-100:    #c2c2c2 !default;
	$gray-200:    #edeff0 !default;
	$gray-300:    #f3f3f3 !default;
	$gray-400:    #ebebeb !default;
	$gray-500:    #ccc !default;
	$black-100:       #25272c !default;
	$blue:        #4782F6 !default;//蓝色
	$blue-100:    #2f71f5 !default;//蓝色-100
	$indigo:      #6610f2 !default;//靛蓝
	$purple:      #6f42c1 !default;//紫色
	$pink:        #e83e8c !default;//粉色
	$red:         #ff3a31 !default;//红色
	$red-100:     #e5352c !default;
	$orange:      #ff6743 !default;//橙色
	$orange-100:  #e55b3c !default;
	$yellow:      #ff7304 !default;//黄色
	$yellow-100:  #e56a05 !default;
	$green:       #87d37b !default;//绿色
	$green-100:   #76ba6c !default;
	$teal:        #20c997 !default;//水鸭色
	$cyan:        #c9d9fc !default;//青色
	
	
	$primary:       $blue !default;//主色
	$primary-100:   $blue-100 !default;
	$auxiliary:     $gray !default;//辅助色
	$success:       $green !default;//成功
	$success-100:   $green-100 !default;
	$info:          $cyan !default;//信息
	$warning:       $yellow !default;//警告
	$warning-100:   $yellow-100 !default;
	$danger:        $red !default;//危险
	$danger-100:        $red-100 !default;
	$light:         $orange !default;//光/亮
	$light-100:     $orange-100 !default;
	$dark:          $black-100 !default;//黑暗的
	$disable:       $gray-500 !default;//禁用
	
	//space间距
	
	$spacing-base:  px2rem(15px) !default;
	$spacing-m:     px2rem(20px) !default;
	$spacing-md:    px2rem(24px) !default;
	$spacing-lg:    px2rem(28px) !default;
	$spacing-lgd:     px2rem(30px) !default;
	$spacing-sm:    px2rem(10px) !default;
	$spacing-smd:   px2rem(5px) !default;
	
	//margin/padding
	$mar-base:        $spacing-base!default;
	$mar-m:           $spacing-m!default;
	$mar-md:          $spacing-md!default;
	$mar-lg:          $spacing-lg!default;
	$mar-lgd:         $spacing-lgd!default;
	$mar-sm:          $spacing-sm!default;
	$mar-smd:         $spacing-smd!default;
	
	$pad-base:        $spacing-base!default;
	$pad-m:           $spacing-m!default;
	$pad-md:          $spacing-md!default;
	$pad-lg:          $spacing-lg!default;
	$pad-lgd:         $spacing-lgd!default;
	$pad-sm:          $spacing-sm!default;
	$pad-smd:         $spacing-smd!default;
	
	$mar-l-base:      $spacing-base!default;
	$mar-l-m:         $spacing-m!default;
	$mar-l-md:        $spacing-md!default;
	$mar-l-lg:        $spacing-lg!default;
	$mar-l-lgd:       $spacing-lgd!default;
	$mar-l-sm:        $spacing-sm!default;
	$mar-l-smd:       $spacing-smd!default;
	
	$pad-l-base:      $spacing-base!default;
	$pad-l-m:         $spacing-m!default;
	$pad-l-md:        $spacing-md!default;
	$pad-l-lg:        $spacing-lg!default;
	$pad-l-lgd:       $spacing-lgd!default;
	$pad-l-sm:        $spacing-sm!default;
	$pad-l-smd:       $spacing-smd!default;
	
	$mar-r-base:      $spacing-base!default;
	$mar-r-m:         $spacing-m!default;
	$mar-r-md:        $spacing-md!default;
	$mar-r-lg:        $spacing-lg!default;
	$mar-r-lgd:       $spacing-lgd!default;
	$mar-r-sm:        $spacing-sm!default;
	$mar-r-smd:       $spacing-smd!default;
	
	$pad-r-base:      $spacing-base!default;
	$pad-r-m:         $spacing-m!default;
	$pad-r-md:        $spacing-md!default;
	$pad-r-lg:        $spacing-lg!default;
	$pad-r-lgd:       $spacing-lgd!default;
	$pad-r-sm:        $spacing-sm!default;
	$pad-r-smd:       $spacing-smd!default;
	
	$mar-t-base:      $spacing-base!default;
	$mar-t-m:         $spacing-m!default;
	$mar-t-md:        $spacing-md!default;
	$mar-t-lg:        $spacing-lg!default;
	$mar-t-lgd:       $spacing-lgd!default;
	$mar-t-sm:        $spacing-sm!default;
	$mar-t-smd:       $spacing-smd!default;
	
	$pad-t-base:      $spacing-base!default;
	$pad-t-m:         $spacing-m!default;
	$pad-t-md:        $spacing-md!default;
	$pad-t-lg:        $spacing-lg!default;
	$pad-t-lgd:       $spacing-lgd!default;
	$pad-t-sm:        $spacing-sm!default;
	$pad-t-smd:       $spacing-smd!default;
	
	$mar-b-base:      $spacing-base!default;
	$mar-b-m:         $spacing-m!default;
	$mar-b-md:        $spacing-md!default;
	$mar-b-lg:        $spacing-lg!default;
	$mar-b-lgd:       $spacing-lgd!default;
	$mar-b-sm:        $spacing-sm!default;
	$mar-b-smd:       $spacing-smd!default;
	
	$pad-b-base:      $spacing-base!default;
	$pad-b-m:         $spacing-m!default;
	$pad-b-md:        $spacing-md!default;
	$pad-b-lg:        $spacing-lg!default;
	$pad-b-lgd:       $spacing-lgd!default;
	$pad-b-sm:        $spacing-sm!default;
	$pad-b-smd:       $spacing-smd!default;
	
	// body-bg
	$body-bg:                   $gray-400 !default;
	
	//font
	$font-base-family:            "Helvetica Neue", Helvetica, STHeiTi, sans-serif !default;
	
	$font-base-color:           $dark !default;//正文文字
	$font-primary-color:        $primary !default;//突出文字
	$font-weak-color:           $gray !default;//辅助色
	$font-danger-color:         $danger !default;//错误用色
	$font-warning-color:        $warning !default;//购买用色
	$font-success-color:        $success !default;//正确用色
	
	$font-size-base:              px2rem(30px) !default;
	$font-size-lg:                px2rem(36px) !default;
	$font-size-sm:                px2rem(24px) !default;
	$font-size-smaller:           px2rem(20px) !default;
	$font-size-lead:              px2rem(18px) !default;
	
	
	$line-height-base:            1.5 !default;
	
	$h1-font-size:                $font-size-lg !default;
	$h2-font-size:                $font-size-base !default;
	$h3-font-size:                $font-size-base  !default;
	$h4-font-size:                $font-size-sm  !default;
	$h5-font-size:                $font-size-smaller  !default;
	$h6-font-size:                $font-size-lead !default;
	
	
	// Links
	$link-color:                  $font-base-color!default;//继承父级颜色
	$link-decoration:             none !default;//没有下划线
	$link-hover-color:            darken($link-color, 15%) !default;//颜色变暗
	$link-hover-decoration:       underline !default;//下划线
	
	// border
	$border-base-width:                1px !default;
	
	//border-color
	$border-base-color:                $gray !default;
	$border-primary-color:             $primary !default;
	$border-warning-color:             $warning !default;
	$border-danger-color:              $danger !default;
	$border-success-color:             $success !default;
	
	
	//Button
	$button-base-width:      px2rem(120px) !default;
	$button-m-width:         px2rem(130px) !default;
	$button-md-width:        px2rem(150px) !default;
	$button-lg-width:        px2rem(190px) !default;
	$button-lgd-width:       px2rem(210px) !default;
	$button-sm-width:        px2rem(90px) !default;
	$button-smd-width:       px2rem(60px) !default;
	
	$button-base-height:     px2rem(50px) !default;
	$button-m-height:        px2rem(56px) !default;
	$button-md-height:       px2rem(60px) !default;
	$button-lg-height:       px2rem(68px) !default;
	$button-lgd-height:      px2rem(70px) !default;
	$button-sm-height:       px2rem(44px) !default;
	$button-smd-height:      px2rem(40px) !default;
	
	$button-default-bg:      $white !default; //默认
	$button-primary-bg:      $primary !default;//突出
	$button-waring-bg:       $warning !default;//警告
	$button-danger-bg:       $danger !default;//危险
	$button-success-bg:      $success !default;//成功
	$button-disable-bg:      $disable !default;//禁用
	$button-light-bg:        $light !default;
	
	$button-primary-ed-bg:      $primary-100 !default;//突出
	$button-waring-ed-bg:       $warning-100 !default;//警告
	$button-danger-ed-bg:       $danger-100 !default;//危险
	$button-success-ed-bg:      $success-100 !default;//成功
	$button-light-ed-bg:        $light-100 !default;
	
	//input
	$input-base-radius:         px2rem(10px) !default;
	$input-base-border:         0 !default;
	$input-pad:                 px2rem(28px) !default;
	
	// Z-index master list
	$zindex-dropdown:                   1000 !default;
	$zindex-sticky:                     1020 !default;
	$zindex-fixed:                      1030 !default;
	$zindex-modal-backdrop:             1040 !default;
	$zindex-modal:                      1050 !default;
	$zindex-popover:                    1060 !default;
	$zindex-tooltip:                    1070 !default;
