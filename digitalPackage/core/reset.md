# reset

##### 定义：

		在HTML标签在浏览器里有默认的样式，例如 p 标签有上下边距，strong标签有字体加粗样式，em标签有字体
	倾斜样式。不同浏览器的默认样式之间也会有差别，例如ul默认带有缩进的样式，在IE下，它的缩进是通过margin
	实现的，而Firefox下，它的缩进是由padding实现的。在切换页面的时候，浏览器的默认样式往往会给我们带来麻
	烦，影响开发效率。所以解决的方法就是一开始就将浏览器的默认样式全部去掉，更准确说就是通过重新定义标签样
	式。“覆盖”浏览器的CSS默认属性。最最简单的说法就是把浏览器提供的默认样式覆盖掉！这就是CSS reset。

##### 重置作用:

		因为浏览器的品种很多，每个浏览器的默认样式也是不同的，比如<button>标签，在IE浏览器、Firefox浏览
	器以及Safari浏览器中的样式都是不同的，所以，通过重置button标签的CSS属性，然后再将它统一定义，就可以
	产生相同的显示效果。
	
### _reset.scss


	 @import "setting";

		html,
		body,
		p,
		pre,
		dl,
		dd,
		h1,
		h2,
		h3,
		h4,
		h5,
		h6,
		blockquote,
		ul,
		ol,
		menu {
		  margin: 0;
		}
		
		input,
		option {
		  padding: 0;
		}
		
		input,textarea{
		  box-shadow:none;
		  -webkit-appearance:none;
		}
		input {
		  border: 0;
		}
		ul,
		ol,
		menu {
		  padding-left: 0;
		  list-style: none;
		}
		
		ns,
		a:hover{
		  text-decoration: none;
		}
		a,ns {
		  cursor: pointer;
		}
		
		i,
		cite,
		dfn,
		em {
		  font-style: normal;
		}
		
		
		del {
		  text-decoration: line-through;
		}
		
		input,
		button,
		textarea,
		select,
		optgroup,
		option {
		  font-family: inherit;
		  font-size: inherit;
		  font-style: inherit;
		  font-weight: inherit;
		  outline: 0;
		}
		
		button {
		  -webkit-appearance: none;
		  border: 0;
		  background: none;
		}
		
		a {
		  -webkit-touch-callout: none;
		}
		
		:focus {
		  outline: 0;
		  -webkit-tap-highlight-color: transparent;
		}
		
		cite,em, i {
		  font-style: normal;
		}
		
		input[type="date"] {
		  text-align: right;
		}
		
		input::-webkit-outer-spin-button,
		input::-webkit-inner-spin-button{
		  -webkit-appearance: none !important;
		  margin: 0;
		}
		
		table {
		  border-collapse: collapse;
		  border-spacing: 0;
		}
		
		caption, th {
		  text-align: left;
		}
		
		fieldset,
		img {
		  border: 0;
		}
