## 简介

轮播效果实现，依赖于jQuery,默认样式为全屏轮播，如有需要可自定义样式。

在线示例：http://yangxiaofu.com/compents/galler/index.html
## 如何使用

1. HTML结构

```html
<div class="page-wrapp">
	<div class="item-wrap">
		<div class="sub-item"></div>
		<div class="sub-item"></div>
		<div class="sub-item"></div>
		<div class="sub-item"></div>
		<div class="sub-item"></div>
	</div>
</div>
```

默认结构为三次，轮播元素为5个，轮播图可放在.sub-item之下，即

```html
<div class="subitem">
	<img src="/my-image.jpg" alt="">
</div>
```
这样就添加了一张图片元素


2. 自定义样式，在main.css之后引入

* 给page-wrapp设宽高

```css
.page-wrapp{
	/*调整位置可在此设置*/
	position: relative;
	/*轮播外层框架宽高设置*/
	width: 500px;
	height: 400px;
}

.page-wrapp .item-wrap{
	/*宽度默认为500%(若有4个子元素，则改为400%)
	高度默认为100%*/
	width: 500%;
}
```

3. 脚本引入

按顺序引入jquery、slider.js,路径可自定义

```javascript
<script src="./js/jquery-2.1.4"></script>
<script src="./js/slider.js"></script>
```

