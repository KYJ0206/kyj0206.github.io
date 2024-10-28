---
title: "[Google Analytics] Google 애널리틱스 시작하기"
excerpt: "Google Analytics 사용법"
categories:
  - Analytics
tags:
  - [Google, Analytics]
toc: true
toc_sticky: true
published: true

date: 2022-03-14
last_modified_at: 2022-03-14
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 구글 애널리틱스 사용법을 포스팅 해 보겠습니다.**</span>

<span style='font-size:1rem'>**지금까지 깃허브 블로그를 만들었고 VScode(에디터)로 작업환경을 만들었습니다.**</span>

<span style='font-size:1rem'>**이제는 블로그 접속자 수를 알 수 있는 구글 애널리틱스를 연동해겠습니다.**</span>

---

### [구글 애널리틱스(Google Analytics)란?] <br>

<a href="https://images.velog.io/images/kyj0206/post/278881e4-1b00-4050-b573-a461b1d00101/123123.jpeg">
![https://images.velog.io/images/kyj0206/post/278881e4-1b00-4050-b573-a461b1d00101/123123.jpeg](https://images.velog.io/images/kyj0206/post/278881e4-1b00-4050-b573-a461b1d00101/123123.jpeg)
</a>

Google <a href='https://analytics.google.com/' target="_blank">Analytics(GA)</a>는, 구글에서 제공하는 무료 웹분석 툴입니다.

구글의 고유한 통계 및 머신러닝 기술로 사이트 및 모바일 애플리케이션 방문자들의 행동 데이터를 분석하고,

마케팅의 실적이나 웹사이트의 경험을 개선할 수 있도록 도와주는 도구입니다.

GA는 ‘전자상거래 플랫폼’, ‘모바일 애플리케이션 ‘그리고 ‘온라인 판매 시점 시스템’ 등 인터넷에 연결된 시스템의 데이터를 보고할 수 있습니다.

쉽게말해 어떤 사용자가 우리 웹사이트를 방문하는지, 어떤 경로를 통해 방문 했는지, 웹사이트에서 어떤 행동을 보이는지에 대한 흔적을 분석한 데이터를 손쉡게 보여주는 도구입니다.

### [구글 애널리틱스의 장점]

> 1. 무료 서비스 제공
>
> - 구글 계정만 있다면, 누구나 사용가능하다
>
> 2. 구글의 광고 서비스와의 연동
>
> - 구글 애널리틱스에서 사용자의 특정조건을 이용하여, 광고계정에서 리마케팅 캠페인을 만들 수 있다!
>
> 3. 다양한 분석 기능을 제공
>
> - (출처: <a href='https://blog.naver.com/PostView.nhn?blogId=sanalytica&logNo=222195954338' target="_blank">Funnel Analysis</a>, <a href='https://support.google.com/analytics/answer/3125360?hl=ko#zippy=%2C%EC%9D%B4-%EB%8F%84%EC%9B%80%EB%A7%90%EC%97%90-%EB%82%98%EC%99%80-%EC%9E%88%EB%8A%94-%EB%82%B4%EC%9A%A9%EC%9D%80-%EB%8B%A4%EC%9D%8C%EA%B3%BC-%EA%B0%99%EC%8A%B5%EB%8B%88%EB%8B%A4' target="_blank">Segment Analysis</a> 등)

### [구글 애널리틱스 시작하기]

#### 1.구글 애널리틱스 접속

구글 애널리틱스 사이트에 접속 해 줍니다.

> <a href='https://analytics.google.com/analytics/web/provision/?authuser=1#/provision' target="_blank">![GitHub Logo](https://images.velog.io/images/kyj0206/post/2a5e61cd-48c1-4f58-b61e-c72da736c44e/mainmain.png)</a>
> link: <a href='https://analytics.google.com/analytics/web/provision/?authuser=1#/provision' target="_blank">analytics.google.com</a>

#### 2.구글 애널리틱스 계정 생성

아래 이미지와 같이 측정시작 버튼을 눌러 계정생성을 시작합니다.

<a href="https://images.velog.io/images/kyj0206/post/051bf9f6-290a-48d6-bb29-a14aa9893dcd/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%205.12.39.png">
![https://images.velog.io/images/kyj0206/post/051bf9f6-290a-48d6-bb29-a14aa9893dcd/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%205.12.39.png](https://images.velog.io/images/kyj0206/post/051bf9f6-290a-48d6-bb29-a14aa9893dcd/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%205.12.39.png)
</a>

계정이름을 설정해주고 넘어가 줍니다.

<a href="https://images.velog.io/images/kyj0206/post/9a98be8c-dd27-4804-8aec-ef9bedf67623/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.02.06.png">
![https://images.velog.io/images/kyj0206/post/9a98be8c-dd27-4804-8aec-ef9bedf67623/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.02.06.png](https://images.velog.io/images/kyj0206/post/9a98be8c-dd27-4804-8aec-ef9bedf67623/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.02.06.png)
</a>

속성이름을 설정하고, 시간을 한국시간으로 설정 해 줍니다.

<a href="https://images.velog.io/images/kyj0206/post/1088150c-c958-4ffa-bfde-17d801ce92e9/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.03.21.png">
![https://images.velog.io/images/kyj0206/post/1088150c-c958-4ffa-bfde-17d801ce92e9/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.03.21.png](https://images.velog.io/images/kyj0206/post/1088150c-c958-4ffa-bfde-17d801ce92e9/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.03.21.png)
</a>

블로그에 맞춰 원하는 설정을 체크 해 줍니다.

<a href="https://images.velog.io/images/kyj0206/post/bdd0472a-76ba-4b60-94c1-99b4c27c28f4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.03.59.png">
![https://images.velog.io/images/kyj0206/post/bdd0472a-76ba-4b60-94c1-99b4c27c28f4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.03.59.png](https://images.velog.io/images/kyj0206/post/bdd0472a-76ba-4b60-94c1-99b4c27c28f4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-14%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%206.03.59.png)
</a>

대한민국으로 설정해여 주고, 약관에 동의해주면 계정설정은 끝납니다.

<a href="https://images.velog.io/images/kyj0206/post/b4cfab82-0ee9-4380-81ee-019d65cfcf42/%E1%84%83%E1%85%A1%E1%84%8B%E1%85%AE%E1%86%AB%E1%84%85%E1%85%A9%E1%84%83%E1%85%B3.png">
![https://images.velog.io/images/kyj0206/post/b4cfab82-0ee9-4380-81ee-019d65cfcf42/%E1%84%83%E1%85%A1%E1%84%8B%E1%85%AE%E1%86%AB%E1%84%85%E1%85%A9%E1%84%83%E1%85%B3.png](https://images.velog.io/images/kyj0206/post/b4cfab82-0ee9-4380-81ee-019d65cfcf42/%E1%84%83%E1%85%A1%E1%84%8B%E1%85%AE%E1%86%AB%E1%84%85%E1%85%A9%E1%84%83%E1%85%B3.png)
</a>

#### 3.구글 애널리틱스 계정 블로그와 연결

먼저 데이터스트림을 만들어주면 되는데 블로그 데이터는 웹입니다. 그러므로,

IOS app / Android app / Wep 중에 웹으로 설정하여 줍니다.

웹 스트림 설정에서는 웹사이트 URL에 자신의 블로그 형식을 입력하고, 스트림 이름은 블로그 이름을 동일하게 넣어줍니다.

이후 스트림 만들기 를 진행해주면 됩니다.

스트림 세부정보에서 측정 ID를 복사해 줍니다.

<a href="https://images.velog.io/images/kyj0206/post/055ea4dd-a6a1-403e-8d6d-5181b28a995e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-18%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2010.38.56.png">
![https://images.velog.io/images/kyj0206/post/055ea4dd-a6a1-403e-8d6d-5181b28a995e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-18%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2010.38.56.png](https://images.velog.io/images/kyj0206/post/055ea4dd-a6a1-403e-8d6d-5181b28a995e/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-18%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2010.38.56.png)
</a>

이후 자신의 블로그 \_config.yml파일에서 provider를 google-gtag로 바꾸고 tracking_id에 방금 복사한 측 ID값을 붙여 넣어줍니다.

```css
# Analytics
analytics:
  provider: "google-gtag"  # false (default), "google", "google-universal", "google-gtag", "custom"
  google:
    tracking_id: "G-SZCCGBLH3T"
    anonymize_ip: #false (default)
```

업데이트 내역을 Commit 하여 Push 해주고, 애널리틱스에 접속하여 주면 연동이 된 결과를 확인할 수 있습니다.

<a href="https://images.velog.io/images/kyj0206/post/42cd5a1d-7529-416a-aa43-5d3320ae5097/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-18%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.53.13.png">
![https://images.velog.io/images/kyj0206/post/42cd5a1d-7529-416a-aa43-5d3320ae5097/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-18%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.53.13.png](https://images.velog.io/images/kyj0206/post/42cd5a1d-7529-416a-aa43-5d3320ae5097/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-18%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%202.53.13.png)
</a>

---

<span style='font-size:1rem'> **지금까지 Google Analytics에 대해 포스팅을 통해 배워 보았습니다.** </span><br>
<span style='font-size:1rem'> **애널리틱스를 이용하여, 블로그를 유용하게 관리해 나가시길 바라겠습니다.** </span><br>
<span style='font-size:1rem'> **다음 포스팅은 더 유익한 정보로 찾아뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
