---
title: "[Javascript] Type"
date: 2019-09-16 20:14:00
categories: Javascript
---

### 자바스크립트 내장 타입 7가지
* null 
* undefined 
* boolean
* number
* string
* object
* symbol

<pre><code>
{} === {} //false 
{} == {} //false 
null === undefined //false 
42 === “42” //false 
null == undefined //true 
42 == “42” //true 
true == 1 //true 
false == 0 //true
</code></pre>


* * *

타입은 typeof 연산자로 확인할 수 있음

<pre><code>
typeof null //object 
typeof undefined //undefined 
typeof Symbol() //symbol 
typeof Symbol //function
</code></pre>

* typeof가 반환하는 function은 object의 하위 타입임(callable object)
* typeof 연산자의 반환값은 "String"임(typeof typeof 1 //string)

* * *

### "변수는 타입이 없다"
변수는 값을 가질 뿐 
값에는 타입이 존재함

