---

layout: post

title: "Node와 Element Node 그리고 childNodes, children"

---
```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
    <script src="index.js"></script>
</head>
<body>
	<section id="section4">
		<h1>Ex4 : childNodes를 이용한 노드 선택</h1>
		<div class="box">
			<input />
			<input />
		</div>
	</section>
	<hr/>
</body>
</html>
```
```javascript
//Ex4 : childeNodes를 이용한 노드 선택
window.addEventListener("load", function () {
    var section4 = document.querySelector("#section4");
    //var inputs = section4.querySelectorAll("input");
    var box = section4.querySelector(".box");
    var input1 = box.children[0]//.childNodes[0];←빈공백까지 node라고 생각한다.
    var input2 = box.children[1];

    input1.value = "hello";
    input2.value = "okay";

});
```