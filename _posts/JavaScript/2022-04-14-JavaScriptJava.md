---
title: "[JavaScript]와 Java의 차이점과 특징"
excerpt: "JavaScript와 Java의 다른점을 알아보자"
categories:
  - JavaScript
tags:
  - [JavaScript]
toc: true
toc_sticky: true
published: true

date: 2022-04-14
last_modified_at: 2022-04-14
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 JavaScript와 Java의,**</span> <br>
<span style='font-size:1rem'>**차이점과 특징을 자세히 알아 보겠습니다.**</span>

---

### [ JavaScript ≠ Java ] <br>

<a href="https://velog.velcdn.com/images/kyj0206/post/53a043e7-b54e-4492-b1bf-b6b248c8fd5e/image.webp">
![https://velog.velcdn.com/images/kyj0206/post/53a043e7-b54e-4492-b1bf-b6b248c8fd5e/image.webp](https://velog.velcdn.com/images/kyj0206/post/53a043e7-b54e-4492-b1bf-b6b248c8fd5e/image.webp)
</a>
이미지 출처:<a href="https://www.boldare.com/blog/java-vs-javascript-what-is-the-difference/"> BOLDARE</a>

먼저 JavaScript와 Java 는 이름만 두고 보면 두 개발 언어가 관련이 있다고 생각됩니다.<br>
하지만 두 언어의 차이점을 확인해 보면 명확이 다른 언어라고 알수 있습니다.

그렇다면, 왜 이름만 비슷한 서로 완전히 다른 개발 언어인지,<br>
자바와 자바스크립트가 정확하게 어떻게 다른지에 대해 포스팅 하겠습니다.<br><br>

#### 1. 탄생 배경<br>

먼저 자바와 자바스크립트의 탄생 배경을 알면<br>
자바와 자바스크립트 언어의 특성에 대한 이해가 쉬워질 것입니다.

##### 자바 (JAVA)<br>

<a href="https://velog.velcdn.com/images/kyj0206/post/b20d89d7-d4f7-401f-8126-babaa8cfd664/image.webp">
![https://velog.velcdn.com/images/kyj0206/post/b20d89d7-d4f7-401f-8126-babaa8cfd664/image.webp](https://velog.velcdn.com/images/kyj0206/post/b20d89d7-d4f7-401f-8126-babaa8cfd664/image.webp)
</a>

자바는 가전 제품에 들어갈 소프트웨어를 만들기 위해 탄생했습니다.<br>
선 마이크로 시스템즈사의 제임즈 고슬링(James Gosling)이라는 사람이 개발하였습니다.

당시 특정 컴퓨터 대해 컴파일 해야하는 컴퓨터 언어인 C언어의 문제점과 가전제품의<br>
완벽한 소프트웨어를 개발하다가 기존 C언어의 불필요한 부분과 문제를 제거한<br>
새로운 언어를 개발하게 되었는데, 이것이 바로 지금의 자바 입니다.

자바라는 이름은 지역의 어느 커피점 안에서 얻었습니다. <br>
그래서 지금은 웹 페이지에서 항상 끓고 있는 커피의 상징을 볼 수 있다.
<br><br>

##### 자바스크립트 (JAVASCRIPT)

<a href="https://velog.velcdn.com/images/kyj0206/post/4b5a62f0-99fb-4943-9d32-76f7f37b4793/image.png">
![https://velog.velcdn.com/images/kyj0206/post/4b5a62f0-99fb-4943-9d32-76f7f37b4793/image.png](https://velog.velcdn.com/images/kyj0206/post/4b5a62f0-99fb-4943-9d32-76f7f37b4793/image.png)
</a>
1995년, 당시 네스케이프사의 네비게이터가 웹브라우저 시장을 지배하고 있었는데,<br>
네스케이프는 HTML페이지에 경량의 프로그램 언어를 통하여 <br>
인터렉티브한 것을 추가 하기로 결정했습니다.
 
그래서 Brendan Erich를 고용했고, 그는 10일 만에 언어를 만들었습니다.

그 언어의 이름은 초기에 ‘모카’였고, 9월 ‘라이브스크립트’로 이름을 변경하였습니다.<br>
그해 12월 네스케이프는 최종적으로 이름을 ‘자바스크립트’라고 결정하였습니다.<br><br>

#### 2. 차이점<br>

|               **JavaScript**                |               **Java**               |
| :-----------------------------------------: | :----------------------------------: |
|           객체지향 스크립트 언어            |       객체지향 프로그래밍 언어       |
|                타입 명시 (X)                |            타입 명시 (O)             |
| 프로토타입(prototype) 기반의 객체 지향 언어 | 해당요소의 사용자 정의 특성값을 삽입 |
