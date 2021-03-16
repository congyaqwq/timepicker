## 基于jquery的一款时间选择器组件，每次重新打开时间会重置
	
	
### 主要思路
	定义全局变量year，month，day，使用函数对其进行操作，最终达到展示效果
	
### 封装组件方法
```javascript
	$.extend({
		timePickerCom: function(name) {
			...
		}
	)}
	
```
### 使用方法
```html
	<!-- 先调用jquery再导入组件 -->
	<!DOCTYPE html>
	<html>
	<head>
		<meta charset="utf-8">
		<title>调用组件</title>
		<link rel="stylesheet" type="text/css" href="日期选择器.css">
		<script type="text/javascript" src="./jquery.js"></script>
		<script type="text/javascript" src="./日期选择器.js"></script>
	</head>
	<body>
		<div id="app"></div>
	</body>
	</html>
```

### 三个版本
	1. 第一个，没有星期
	2. 第二个，有星期，没有上一月下一月
	3. 第三个，比较标准的7*6格式
