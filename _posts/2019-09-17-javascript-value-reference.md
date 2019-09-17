---
title: "[Javascript] 값과 레퍼런스"
date: 2019-09-17 21:24:00 -0700
categories: javascript
---

##### 값을 복사하는 방식

null, undefined, string, number, boolean, symbol

 
* * *
 

##### 레퍼런스를 복사하는 방식

객체(배열 포함), 함수

변수가 아닌 값 자체를 가리키므로, 가리키는 대상의 값을 바꿀수는 없음

<pre><code>var a = [1, 2, 3];
var b = a;

a; //[1, 2, 3]
b; //[1, 2, 3]

b = [3, 4, 5];

a; //[1, 2, 3]
b; //[3, 4, 5]
</code></pre>
