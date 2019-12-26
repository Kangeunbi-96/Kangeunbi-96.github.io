---

layout: post

title: "window 플랫폼을 이용한 대화 parseInt, alert, prompt, confirm"

---
###### *window.alert() : 경고창을 띄울 때 사용한다. window 객체는 생략 가능하다. alert("경고 메세지");
###### *window.prompt() : 질의응답 창을 나타낼 때 사용한다. window 객체는 생략 가능하다. prompt("내용","입력창 default 값"");
###### *window.confirm() : 확인 또는 취소 창을 나타낼 때 사용한다.  window 객체는 생략 가능하다. confirm("내용"); confirm() 함수로 띄운 창에서 확인 버튼을 클릭하면 결과값으로 true를 반환하고 취소 버튼을 클릭하면 false를 반환한다. 
###### *parseInt() : 문자열을 정수로 바꾸는 함수이다. parseInt("abc"); // Returns NaN parseInt("12abc"); // Returns 12