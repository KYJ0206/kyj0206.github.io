---
title: "[JavaScript]의 개념과 기본"
excerpt: "JavaScript란?"
categories:
  - JavaScript
tags:
  - [JavaScript]
toc: true
toc_sticky: true
published: true

date: 2022-04-11
last_modified_at: 2022-04-11
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 JavaScript의 개념과 기본을**</span> <br>
<span style='font-size:1rem'>**간단하게 알아보는 포스팅을 진행하겠습니다.**</span>

<span style='font-size:1rem'>**상세포스팅으로 별도의 포스팅을 진행할 예정이니,**</span><br>
<span style='font-size:1rem'>**이번 포스팅은 가볍게 이해만 하고 지나가셔도 무방합니다.**</span>

---

### [JavaScript] 란?<br>

<a href="https://velog.velcdn.com/images/kyj0206/post/1cbf6dd7-87d2-409c-a420-8145b4f937ce/image.jpeg">
![https://velog.velcdn.com/images/kyj0206/post/1cbf6dd7-87d2-409c-a420-8145b4f937ce/image.jpeg](https://velog.velcdn.com/images/kyj0206/post/1cbf6dd7-87d2-409c-a420-8145b4f937ce/image.jpeg)
</a>

자바스크립트는 복잡한 무언가(주기적으로 내용이 갱신되는 기능이나 능동적인 지도, 변화하는 2D/3D 그래픽, 동영상 등)를 웹페이지에 적용할 수 있게 하는 스크립트 혹은 프로그래밍 언어입입니다.

자바스크립트는 표준 웹 기술이라는 레이어 케이크에서 세번째 층이라고 볼 수 있습니다.

- <a href="https://kyj0206.github.io/html/HTML/">HTML</a>은 제공할 웹 컨텐츠의 구조와 의미를 문단, 제목, 표, 삽입 이미지, 동영상 등으로 정의하고 부여하는 마크업 언어입니다.

- <a href="https://kyj0206.github.io/css/CSS/">CSS</a>는 배경색, 폰트 등의 레이아웃등을 지정하여 HTML 컨텐츠를 꾸며주는 스타일 규칙 언어입니다.

- JavaScript는 동적으로 컨텐츠를 바꾸고, 멀티미디어를 다루고, 움직이는 이미지 그리고 꽤나 많은 다른 일들을 할 수 있는 스크립트 언어입니다.
  <br><br>

#### JavaScript 의 어원<br>

자바스크립트는 1995년에 넷스케이프(Netscape)의<br>
브렌던 아이크(Brendan Eich)에 의해 만들어졌습니다.

처음에는 모카(Mocha)라는 이름으로 개발되었으나, 그 후에 라이브스크립트(LiveScript), 최종적으로는 자바스크립트(JavaScript)라는 이름으로 변경되었습니다.

<br>

#### JavaScript 의 특징<br>

- 자바스크립트는 객체 기반의 스크립트 언어입니다.

- 자바스크립트는 동적이며, 타입을 명시할 필요가 없는 인터프리터 언어입니다.

  > 인터프린터 언어 :
  >
  > C언어와 같은 언어는 소스 파일을 작성한 후, 해당 파일을 컴파일(compile)하여 사용자가 실행할 수 있는 실행 파일(.exe)로 만들어 사용합니다.
  >
  > 인터프리터 언어는 이러한 컴파일 작업을 거치지 않고, 소스 코드를 바로 실행할 수 있는 언어를 의미합니다.
  >
  > 자바스크립트는 웹 브라우저에 포함된 자바스크립트 인터프리터가 소스 코드를 직접 해석하여 바로 실행해 줍니다.

- 자바스크립트는 객체 지향형 프로그래밍과 함수형 프로그래밍을 모두 표현할 수 있습니다.

<br>

#### JavaScript 표준안<br>

<a href="https://ko.wikipedia.org/wiki/ECMA%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8">ECMAScript:</a>
넷스케이프가 인터넷 상의 다양한 스크립트 언어를 하나로 묶기 위해 제시한 표준안.

이 스펙을 구현한 JavaScript 구현체로는 구글의 V8 엔진, 모질라의 SpiderMonkey, Microsoft의 Chakra 등이 있습니다.

실제로 JavaScript에만 적용되는 표준안이 아니라, Internet Explorer의 JScript나 Adobe Flash ActionScript의 표준이기도 합니다.

현재는 ECMAScript 2021의 표준 (12판)까지 나와있으며, 현재는 Internet Explorer등의 구형 브라우저를 제외하고는 ECMAScript 2016 표준까지는 적당히 구현이 되어있는 상태입니다. 또한,
구현이 안된 브라우저를 지원하기 위해서 Babel 등의 Transpiler를 사용해서 ECMAScript 2015 이상의 기능을 어느 정도 사용할 수 있습니다.

<br>

#### JavaScript ≠ Java<br>

JavaScript와 Java는 그 이름만 놓고 보면 서로 관련이 있는 언어로 생각되기 쉽습니다.<br>
하지만 두 언어는 서로 직접적인 관련은 없으며, 비슷한 점보다는 다른 점이 훨씬 많습니다.<br>
문법상 비슷한 부분은 두 언어의 문법이 모두 C언어를 기반으로 만들어졌기 때문입니다.

이번 포스팅에서는 간단한 차이점만 아래 표를 통해 표기 하겠습니다.

상세한 차이점과 특징은 상세 포스팅을 통해 포스팅 하겠습니다.

|               **JavaScript**                |               **Java**               |
| :-----------------------------------------: | :----------------------------------: |
|               인터프리터 언어               |             컴파일 언어              |
|                타입 명시 (X)                |            타입 명시 (O)             |
| 프로토타입(prototype) 기반의 객체 지향 언어 | 해당요소의 사용자 정의 특성값을 삽입 |

---

<span style='font-size:1rem'> **지금까지 JavaScript란 무엇인지 포스팅 해 보았습니다.** </span><br>

<span style='font-size:1rem'> **앞으로 JavaScript의 기능과 적용방법을,** </span><br>
<span style='font-size:1rem'> **상세 포스팅으로 진행 해 보겠습니다.** </span><br>

<span style='font-size:1rem'> **감사합니다!** </span>
