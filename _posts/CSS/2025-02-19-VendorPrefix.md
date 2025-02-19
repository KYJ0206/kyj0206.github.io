---
title: "[ VendorPrefix ]란 무엇인가요?"
excerpt: "벤더 프리픽스란 무엇인지 알아보자"
categories:
  - CSS
tags:
  - [CSS, VendorPrefix]
toc: true
toc_sticky: true
published: true

date: 2025-02-19
last_modified_at: 2025-02-19
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 CSS3표준안으로 확정되기 이전이나,**</span> <br>
<span style='font-size:1rem'>**브라우저 개발사가 실험적으로 제공하는 기능을 사용하기 위해서는,**</span> <br>
<span style='font-size:1rem'>**벤더 프리픽스(Vendor Prefix)를 사용하게 됩니다.**</span>

<span style='font-size:1rem'>**지금부터 자세히 설명 드릴테니,**</span> <br>
<span style='font-size:1rem'>**천천히 이해하며 진행해 주시면 감사하겠습니다.**</span>

---

### [ 벤더 프리픽스(Vendor Prefix) 란? ] <br>

<a href="/assets/images/VendorPrefix.png">
![/assets/images/VendorPrefix.png](/assets/images/VendorPrefix.png)
</a>

벤더 프리픽스란 주요 웹 브라우저(Chrome, Firefox, IE, Opera, Safari...) <br>
공급자가 새로운 실험적인 기능을 제공할 때 이전 버전의 웹 브라우저에 그 사실을 알려주기 위해 사용하는 접두사(prefix)를 의미한다.

### [ 웹 브라우저별 벤더 프리픽스 ] <br>

| 브라우저 (Browser)    | 벤더프리픽스 (VendorPrefix)     |
|---------------------|-----------------------------|
| IE or Edge          | -ms-                        |
| Chrome              | -webkit-                    |
| Safari              | -webkit-                    |
| Firefox             | -moz-                       |
| Opera               | -o-                         |

### [ 사용방법 ] <br>

```css
.gradientBox {
  <!-- gradient 속성을 지원하지 않는 모든 브라우저를 위한 코드 -->
  background: yellow; 
  <!-- 크롬과 사파리 4.0 이상을 위한 코드 -->         
  background: -webkit-linear-gradient(yellow, black); 
  <!-- 파이어폭스 3.6 이상을 위한 코드 -->
  background: -moz-linear-gradient(yellow, black);  
  <!-- 익스플로러 10.0 이상을 위한 코드 -->  
  background: -ms-linear-gradient(yellow, black); 
  <!-- 오페라 10.0 이상을 위한 코드 -->    
  background: -o-linear-gradient(yellow, black);
  <!-- CSS 표준 문법 코드 -->     
  background: linear-gradient(yellow, black);         
}
```
> CSS 표준 문법 코드는 벤더 프리픽스(vendor prefix)로 작성된 코드가 모두 나오고 난 후에 나와야만, 벤더 프리픽스가 포함된 코드가 정상적으로 동작할 수 있습니다.

> CSS 표준안으로 적용되거나, 버전에 따라 벤더 프리픽스가 필요 없을수 있습니다.

### [ Prefix free ]

벤더 프리픽스를 생략할 수 있게 도와주는 플러그인 입니다.
라이브러리 사용으로 밴더프리픽스 사용으로 코드의 가독성및 번거로움을 방지할수 있습니다.

#### Prefixfree 공식홈페이지
[Prefixfree 공식 홈페이지](https://projects.verou.me/prefixfree/)<br>
#### Prefixfree 깃허브
[Prefixfree 깃허브](https://github.com/LeaVerou/prefixfree)

<br>

---

<br>

<span style='font-size:1rem'> **지금까지 Zero Runtime CSS-in-JS에 대해 포스팅을 하였습니다.** </span><br>

<span style='font-size:1rem'> **도움이 되는 포스팅이었길 바랍니다.** </span><br>

<span style='font-size:1rem'> **다음 포스팅은 더 유익한 정보로 찾아뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
