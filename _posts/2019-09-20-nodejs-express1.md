---
title: "[Node.js] express로 웹서버 만들기 1"
date: 2019-09-20 22:25:00 -0700
categories: node.js javascript
---

##### express 모듈설치

터미널에서 노드 패키지 관리자를 통해 익스프레스를 설치함

<pre><code>npm install express --save</code></pre>


##### 모듈을 불러 오기

<pre><code>const express = require(‘express’);</code></pre>


##### 객체생성

<pre><code>const app = express();</code></pre>


* app객체의 주요 메소드
  * set(name, value) : 서버 설정을 위한 속성 지정
  * get(name) : set으로 지정한 속성을 가져옴
  * use([path,]function[,function…]) : 미들웨어를 등록
  * get([path,]function) : 특정 패스로 요청된 정보 처리


##### app.set() 메소드로 포트를 설정함
<pre><code>app.set(‘port’, 3000) //3000번 포트 설정
app.get(‘port’) //설정한 포트를 가져옴
</code></pre>


