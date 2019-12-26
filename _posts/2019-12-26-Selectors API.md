---

layout: post

title: "Selectors API"

---
###### Document.querySelector란?
###### - Document.querySelector()는 제공한 선택자 또는 선택자 뭉치와 일치하는 문서 내 첫 번째 Element를 반환한다. 일치하는 요소가 없으면 null을 반환한다.
###### - 선택자를 만족하는 모든 요소의 목록이 필요하다면 querySelectorAll()을 사용한다.

```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
    <script src="index.js"></script>
</head>
<body>
	<section id="section3">
		<h1>Ex3 : Selectors API Level1</h1>
		<div>
			<input name="x" type="text" value="0" dir="rtl">
			+
			<input class="txt-y" type="text" value="0" name="" dir="rtl">
			<input class="btn-add" type="button" value="=" name="" dir="rtl">
			<input class="txt-sum" type="text" value="0" name="" dir="rtl">
		</div>
	</section>
	<hr/>
</body>
</html>
```
```javascript
//Ex3 : Selectors API Level1
window.addEventListener("load", function () {
    var section3 = document.getElementById("section3");
    var txtX = section3.querySelector("input[name = 'x']");
    var txtY = section3.querySelector(".txt-y");
    var btnAdd = section3.querySelector(".btn-add");
    var txtSum = section3.querySelector(".txt-sum");

    btnAdd.onclick = function () {
        var x = parseInt(txtX.value);
        var y = parseInt(txtY.value);

        txtSum.value = x + y;
    };
});
```