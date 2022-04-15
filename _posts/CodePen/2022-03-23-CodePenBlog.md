---
title: "[CodePen] 블로그에 CodePen Embed하는 방법"
excerpt: "CodePen Embed하는법"
categories:
  - CodePen
tags:
  - [Jekyll, Blog, CodePen]
toc: true
toc_sticky: true
published: true

date: 2022-03-23
last_modified_at: 2022-03-23
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**해당 포스팅은 Jekyll 블로그에서 CodePen을 추가하는 방법에 대한 설명입니다.**</span>

<span style='font-size:1rem'>**앞으로의 포스팅에서 이해를 돕기 위해 CodePen을 적용 할 것입니다.**</span>

<span style='font-size:1rem'>**실시간 코드에디터인 CodePen을 알아보고 Html, Css, Js을 손쉽게 CodePen으로 이용하는 방법을 포스팅 하겠습니다.**</span>

---

### [CodePen 이란?] <br>

<a href="https://images.velog.io/images/kyj0206/post/259b5b89-0765-4464-9ca9-41047719ef2e/codepen.png">
![https://images.velog.io/images/kyj0206/post/259b5b89-0765-4464-9ca9-41047719ef2e/codepen.png](https://images.velog.io/images/kyj0206/post/259b5b89-0765-4464-9ca9-41047719ef2e/codepen.png)
</a>

CodePen은 Web_Developer를 위한 Online_Compiler입니다.

쉽게말해 웹 개발자를 기준으로 만들어지다 보니 웹언어에 최적화 되어있다고 볼 수 있으며, 가장 좋은 점은 소스코드를 적용해 결과를 한번에 볼 수 있다는 장점이있습니다.

간단하게 codepen을 직접 블로그에 Embed해 보았습니다.

<iframe height="300" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/kyj0206/embed/yLpVaXa?default-tab=html%2Cresult" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/kyj0206/pen/yLpVaXa">
  Untitled</a> by K.Y.J (<a href="https://codepen.io/kyj0206">@kyj0206</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe><br>
이렇게 적용할 수 있고, 적용 방법 또한, 어렵지 않으니 천천히 진행해 보겠습니다.

### [Codepen Embed 방법]

#### 1. 아래 링크를 통해 Codepen에 접속

[ Link : <a href="https://codepen.io/trending" target="_blank">Codepen ]</a>

#### 2. 계정 생성 및 로그인 진행

우측 상단의 Sign Up 또는 Log In 버튼을 이용하여 진행해 줍니다.<br>

<a href="https://images.velog.io/images/kyj0206/post/b6e9efe5-8bba-4559-8018-b50df6463b3a/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.44.02.png">
![https://images.velog.io/images/kyj0206/post/b6e9efe5-8bba-4559-8018-b50df6463b3a/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.44.02.png](https://images.velog.io/images/kyj0206/post/b6e9efe5-8bba-4559-8018-b50df6463b3a/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.44.02.png)
</a>

GitHub 계정 으로 쉽게 연동가능 합니다.

<a href="https://images.velog.io/images/kyj0206/post/3ded2397-8c5e-44cb-934f-d57ff26a8d6a/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.08.47.png">
![https://images.velog.io/images/kyj0206/post/3ded2397-8c5e-44cb-934f-d57ff26a8d6a/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.08.47.png](https://images.velog.io/images/kyj0206/post/3ded2397-8c5e-44cb-934f-d57ff26a8d6a/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.08.47.png)
</a>

#### 3. New Pen을 생성

우측 상단 스마일 아이콘은 누르면 아래 이미지와 같은 창을 볼 수 있습니다.<br>
New Pen 을 클릭해서 새로운 Pen을 만들어 줍니다.

<a href="https://images.velog.io/images/kyj0206/post/5e6c1e53-2f01-4e82-8d3d-fe5353f6330e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.18.46.png">
![https://images.velog.io/images/kyj0206/post/5e6c1e53-2f01-4e82-8d3d-fe5353f6330e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.18.46.png](https://images.velog.io/images/kyj0206/post/5e6c1e53-2f01-4e82-8d3d-fe5353f6330e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.18.46.png)
</a>

#### 4. 간단한 코드 작성 후 저장

상단의 [ Save ] 버튼 or [ Ctrl+S ] 으로 저장을 해줍니다.

<a href="https://images.velog.io/images/kyj0206/post/7a63a428-bdb7-4203-b60e-2a881b683f8b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.48.44.png">
![https://images.velog.io/images/kyj0206/post/7a63a428-bdb7-4203-b60e-2a881b683f8b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.48.44.png](https://images.velog.io/images/kyj0206/post/7a63a428-bdb7-4203-b60e-2a881b683f8b/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.48.44.png)
</a>

#### 5. CodePen Embed

우측 하단의 Embed 버튼 클릭후 Iframe 탭으로 이동하여 소스 코드 복사해 줍니다.

<a href="https://images.velog.io/images/kyj0206/post/b5e1823f-d7f4-45ae-9421-6e5b38992fe1/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.50.06.png">
![https://images.velog.io/images/kyj0206/post/b5e1823f-d7f4-45ae-9421-6e5b38992fe1/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.50.06.png](https://images.velog.io/images/kyj0206/post/b5e1823f-d7f4-45ae-9421-6e5b38992fe1/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.50.06.png)
</a>

#### 6. 블로그 포스팅 페이지에 적용

복사한 소스코드를 블로그 포스팅 으로 옮겨줍니다.<br>
Local서버로 확인 결과,아래 이미지와 같이 정상적으로 화면에 출력되어 집니다.

<a href="https://images.velog.io/images/kyj0206/post/62695d60-96e3-4e30-a82d-12239d2dcd65/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.51.17.png">
![https://images.velog.io/images/kyj0206/post/62695d60-96e3-4e30-a82d-12239d2dcd65/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.51.17.png](https://images.velog.io/images/kyj0206/post/62695d60-96e3-4e30-a82d-12239d2dcd65/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-23%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.51.17.png)
</a>

마지막으로 Commit 하여 Push 해주고 확인해 주면 끝 입니다.

---

<span style='font-size:1rem'> **지금까지 블로그에서 CodePen을 추가하는 방법을 배워 보았습니다.** </span><br>

<span style='font-size:1rem'> **CodePen을 접목하여,** </span><br>
<span style='font-size:1rem'> **앞으로 블로그를 멋지게 관리해 보세요.** </span><br>

<span style='font-size:1rem'> **다음 포스팅은 더 유익한 정보로 찾아뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
