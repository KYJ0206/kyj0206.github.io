---
title: "[ 제로 런타임 css ]란 무엇인가요?"
excerpt: "Zero Runtime CSS-in-JS는 무엇인지 알아보자"
categories:
  - CSS
tags:
  - [CSS, CSS-in-JS, Zero Runtime]
toc: true
toc_sticky: true
published: true

date: 2025-01-16
last_modified_at: 2025-01-16
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 CSS 의 동작 방식인 CSS-in-JS의 단점을 보완하기 위해**</span> <br>
<span style='font-size:1rem'>**등장한 제로 런타임 CSS에 대해 알아보겠습니다.**</span>

<span style='font-size:1rem'>**자세히 설명 드릴테니,**</span> <br>
<span style='font-size:1rem'>**천천히 이해하며 진행해 주시면 감사하겠습니다.**</span>

---

### [ 제로 런타임 CSS 란? ] <br>

제로 런타임 CSS는 CSS-in-JS의 단점을 보완하기 위해 등장한 방식입니다. 

기존에 많이 쓰이던 CSS-in-JS 방식은 스타일을 컴포넌트 안에서 작성해서 동적으로 생성합니다. 이러한 방식은 런타임에서 CSS를 만들다 보니 성능 문제가 생길 가능성이 있습니다.

쉽게 말해 스타일을 런타임에 적용하지 않고, 빌드 타임에 CSS를 생성하여 사용자가 페이지를 로드할 때 이미 최적화된 CSS를 제공하는 방식입니다.

### [ Zero-Runtime의 장점 ]

- 성능 향상: 런타임에 스타일을 생성하지 않고 빌드 시점에 CSS를 생성하기 때문에 페이지 로딩 시 불필요한 계산이 줄어들어 성능이 개선됩니다.
- 최적화된 스타일: 빌드 타임에 사용되지 않는 스타일을 제거하여 최종 CSS 파일의 크기를 줄이고, 브라우저의 렌더링 성능을 높입니다.
- 유지보수 용이: 컴포넌트 기반의 개발을 지원하며, 각 컴포넌트에 필요한 스타일을 독립적으로 관리할 수 있어 코드의 가독성이 향상됩니다.
- 서버 컴포넌트 호환성: 서버에서 미리 생성된 CSS를 클라이언트에 전달함으로써 초기 로딩 속도를 향상시킵니다.

### [ Zero-Runtime의 단점 ]

- 런타임에서 동적으로 생성해야 하는 스타일을 구현하기가 까다롭습니다. 예를 들어, 사용자 입력값에 따라 스타일이 달라지는 경우엔 추가 로직을 작성해주어야 합니다. 
- 스타일을 빌드 시점에 모두 처리해야 하다 보니, 빌드 시간이 기존보다 길어질 수 있습니다.

### [ CSS-in-CSS, Css-in-JS, Zero Runtime 차이점 ]

#### - CSS-in-CSS(Module css)
각 컴포넌트에 대한 별도의 CSS 파일을 작성하고, 이를 모듈화하여 사용 합니다. <br>
런타임에 CSS가 적용되며, 전체 애플리케이션의 스타일의 크기가 클 경우 성능에 영향을 미칠 수 있습니다.

#### - CSS-in-JS
JavaScript 파일 내에서 CSS를 정의하며 런타임에 스타일을 동적으로 생성 합니다. <br>
CSS-in-CSS 방식과 같이 런타임에 CSS를 생성하기 때문에 성능에 영향이 미칠 수 있습니다.

#### - Zero Runtime CSS-in-JS
스타일을 런타임에 적용하지 않고, 빌드 타임에 CSS를 생성하여 사용자가 페이지를 로드할 때 이미 최적화된 CSS를 제공하는 방식 입니다.

### [ Zero Runtime CSS-in-JS 라이브러리 ]
#### - <a href="https://linaria.dev/" target="_blank">Linaria</a>
TypeScript의 타입 시스템을 활용하여 오류를 줄일 수 있습니다.<br>
CSS-in-JS 문법을 사용하므로 사용 난이도가 적습니다.

#### - <a href="https://vanilla-extract.style/" target="_blank">Vanilla-extract</a>
TypeScript의 타입 시스템을 활용하여 오류를 줄일 수 있습니다.<br>
CSS 변수를 쉽게 사용할 수 있어, 유연한 스타일링이 가능합니다.<br>
정적 스타일링을 통해 런타임 성능이 최적화됩니다.

<br>

---

<br>

<span style='font-size:1rem'> **지금까지 Zero Runtime CSS-in-JS에 대해 포스팅을 하였습니다.** </span><br>

<span style='font-size:1rem'> **도움이 되는 포스팅이었길 바랍니다.** </span><br>

<span style='font-size:1rem'> **다음 포스팅은 더 유익한 정보로 찾아뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
