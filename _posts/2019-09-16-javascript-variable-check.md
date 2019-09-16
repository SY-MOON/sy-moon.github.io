---
title: "[Javascript] 변수 존재여부 체크"
date: 2019-09-16 20:21:00
categories: etc.
---

##### 전역 변수의 존재 여부를 체크 할 때 아래처럼!

<pre><code>if(x) {
	//이렇게 체크하지 말고
}

if(typeof x !== "undefined") {
	//이렇게 안전하게 체크하자
}

if(window.x) {
	//또는 이렇게도 가능하긴 하지만 이 방식은 쓰지말자
  //window객체로만 호출하지 않는 Node와 같은 다중 자바스크립트 환경도 있으니까
}
</code></pre>


* 내장 API기능을 체크할 때도 사용 가능함

