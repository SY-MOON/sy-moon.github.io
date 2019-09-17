---
title: "[Javascript] Number"
date: 2019-09-17 21:14:00 -0700
categories: javascript
---

#### Number

자바스크립트의 숫자 타입 

정수와 부동 소수점 숫자를 포함함

 

큰 숫자의 경우 지수형 표현을 사용함

1E10 = 10,000,000,000

 

 

* toFixed()

        지정한 숫자만큼 소수점 이하 자리까지 숫자를 나타내며 문자열 형태로 반환함

        <pre><code>var num = 12.3;

        num.toFixed(3); //12.300
        </code></pre>
 
 

* toPrecision()

        전체 숫자 자리수를 지정

        <pre><code>var num = 12.3;

        num.toPrecision(5); //12.300
        </code></pre>
       
 

##### NaN(Not a Number)

숫자가 아님 = 유효하지 않은 숫자다, 연산에서 에러가 난다, 정도의 의미

그런데 NaN의 typeof는 숫자임;

NaN은 NaN과 비교불가

 

* isNaN()

        NaN인지 아닌지 확인용

        <pre><code>var x = 12 / 'abc';

        isNaN(x); //true
        </code></pre>

        문제는, 일반적인 문자열을  isNaN()에 넣을 경우도 NaN으로만 인식을 해버림

        ES6부터는 *Number.isNaN()*으로 문제 없이 사용가능!
