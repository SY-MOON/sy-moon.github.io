---
title: "[Javascript] Object.is()"
date: 2019-09-17 21:19:00 -0700
categories: javascript
---

* Object.is()


NaN, -0과 같이 ==, === 연산자로 비교가 어려운 경우 사용함

 
<pre><code>
var x = 123 / 'abc';
var y = -3 * 0;

Object.is(x, NaN); //true
Object.is(y, -0); //true
Object.is(y, 0); //false
</code></pre>
