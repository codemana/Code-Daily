动态创建 HTML 内容
=================

**老方法**

`document.write()` & `innerHTML`

**DOM 方法**

`createElement` 方法

*document.createElement(nodeName)*  插入DOM元素。

`appendChild()` 方法

*parent.appendChild(child)*  把创建的节点插入某个DOM节点。

`crreateTextNode` 方法

*document.createTextNode(text)* 给节点插入内容。

**举例：**
	
	JS:
	
	window.onload = function (){
	var para = document.createElement("p");
	var testdiv = document.getElementById("testdiv");
	testdiv.appendChild(para);
	var txt = document.createTextNode("Hello World!");
	para.appendChild(txt);
	}
	
	HTML:
	
	<div id="testdiv">

	</div>


