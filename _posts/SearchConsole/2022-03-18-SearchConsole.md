---
title: "[ Google SearchConsole ] Google 서치콘솔 시작하기"
excerpt: "Google SearchConsole 사용법"
categories:
  - SearchConsole
tags:
  - [Google, SearchConsole]
toc: true
toc_sticky: true
published: true

date: 2022-03-18
last_modified_at: 2022-03-18
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 구글 서치콘솔 사용법을 포스팅 해 보겠습니다.**</span>

<span style='font-size:1rem'>**애널리틱스와 함께 사용하면 좋은 구글 서치콘솔을 함께 천천히 시작해 봅시다.**</span>

---

### [ 구글 서치 콘솔(Search Console)이란? ] <br>

<a href="https://images.velog.io/images/kyj0206/post/79326a4d-1b39-4f18-9577-d8d4e0c96d21/%E1%84%89%E1%85%A5%E1%84%8E%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB%E1%84%89%E1%85%A9%E1%86%AF.png">
![https://images.velog.io/images/kyj0206/post/79326a4d-1b39-4f18-9577-d8d4e0c96d21/%E1%84%89%E1%85%A5%E1%84%8E%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB%E1%84%89%E1%85%A9%E1%86%AF.png](https://images.velog.io/images/kyj0206/post/79326a4d-1b39-4f18-9577-d8d4e0c96d21/%E1%84%89%E1%85%A5%E1%84%8E%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB%E1%84%89%E1%85%A9%E1%86%AF.png)
</a>

구글 서치콘솔 이란 구글의 전 구글 웹마스터들이 개발한 웹 서비스로서, 웹마스터들이 자신들의 웹사이트의 보이는 부분을 최적화하고 인덱싱 상태를 검사할 수 있게 해줍니다.

구글(Google)로부터 제공되는 정보를 통해서 보다 나은 SEO 대책이 가능해지는 셈이죠. 일전에는 구글 웹 마스터 도구라는 명칭이었지만 현재는 서치 콘솔이라는 타이틀로 변경되어 사용되고 있습니다.

### [ 구글 서치콘솔의 장점 ]

> 1. 구글 애널리틱스를 통해 컨텐츠를 최적화 할 수 있다.
>
> - 내 사이트에 유입되는 사용자가 어떤 키워드, 검색어를 통해 사이트에 방문하는지 알 수 있다.
>
> 2. 구글에 나의 컨텐츠를 표시할 수 있다.
>
> - 크롤링할 사이트맵, URL을 제출해서, 구글이 내 사이트의 최신 버전을 크롤링하도록 색인 생성 범위를 검토해 검색에 더 잘 노출될게 할 수 있다.
>
> 3. 구글검색이 내 페이지를 어떻게 인식하는지 파악할 수 있다.
>
> - URL 검사도구를 사용하여 페이지에 관한 세부적인 크롤링, 색인 생성, 게재 정보를 Google 색인에서 쉽게 확인할 수 있다.

### [ 구글 서치콘솔 시작하기 ]

#### 1.Google Search Console에 사이트 등록

- 1 ) <a href="https://search.google.com/search-console/welcome?hl=ko" target="_blank">Google Search Console</a>에 접속합니다.
- 2 ) 속성 추가를 누릅니다.
- 3 ) Github io 주소를 입력하고 계속을 누릅니다.

<a href="https://images.velog.io/images/kyj0206/post/99718824-cb68-4900-806f-5c4bd8e8f596/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2011.25.41.png">
![https://images.velog.io/images/kyj0206/post/99718824-cb68-4900-806f-5c4bd8e8f596/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2011.25.41.png](https://images.velog.io/images/kyj0206/post/99718824-cb68-4900-806f-5c4bd8e8f596/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2011.25.41.png)
</a>

- 4 ) 해당 페이지의 소유권을 확인하는 절차를 진행합니다. 여러 확인 방법중 저는 HTML태그를 이용하여 진행 해 보겠습니다.

<a href="https://images.velog.io/images/kyj0206/post/62b23d41-031a-4313-a1dc-53417ab66bfa/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2011.44.06.png">
![https://images.velog.io/images/kyj0206/post/62b23d41-031a-4313-a1dc-53417ab66bfa/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2011.44.06.png](https://images.velog.io/images/kyj0206/post/62b23d41-031a-4313-a1dc-53417ab66bfa/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2011.44.06.png)
</a>

- 5 ) \_config.yml 에서 위 이미지의 content 내용을 복사하여 아래 항목에 입력해 줍니다.

```css
# SEO Related
google_site_verification: MSlec-s9ul06lFCiePy5m4gkOoGMJ8j6ObqX8TdKeXE
bing_site_verification:
yandex_site_verification:
naver_site_verification:
```

- 6. 정상적으로 업로드 되었다면 소유권이 확인되었다는 창을 볼 수 있습니다.

<a href="https://images.velog.io/images/kyj0206/post/a703e080-5611-46f2-9ad7-dd83315e42d4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-28%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%2012.19.51.png">
![https://images.velog.io/images/kyj0206/post/a703e080-5611-46f2-9ad7-dd83315e42d4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-28%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%2012.19.51.png](https://images.velog.io/images/kyj0206/post/a703e080-5611-46f2-9ad7-dd83315e42d4/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-28%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%2012.19.51.png)
</a>

#### 2.sitemap.xml 생성

- 1 ) \_config.yml 파일에 url 속성에 자기의 블로그 이름이 들어가 있는지 확인합니다.
- 2 ) sitemap.xml 파일을 자기 github.io root 경로에 생성합니다.
- 3 ) 아래 내용을 sitemap.xml에 추가합니다.

```ruby
---
layout: null
---
< ?xml version="1.0" encoding="UTF-8"? >
< urlset xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.sitemaps.org/schemas/sitemap/0.9 http://www.sitemaps.org/schemas/sitemap/0.9/sitemap.xsd" xmlns="http://www.sitemaps.org/schemas/sitemap/0.9" >
  { % for post in site.posts % }
    < url >
      < loc >{{ site.url }}{{ post.url }}< /loc >
      { % if post.lastmod == null % }
        < lastmod >{{ post.date | date_to_xmlschema }}< /lastmod >
      { % else % }
        < lastmod >{{ post.lastmod | date_to_xmlschema }}< /lastmod >
      { % endif % }

      { % if post.sitemap.changefreq == null % }
        < changefreq >weekly< /changefreq >
      { % else % }
        < changefreq >{{ post.sitemap.changefreq }}< /changefreq >
      { % endif % }

      { % if post.sitemap.priority == null % }
          <priority>0.5</priority>
      { % else % }
        < priority >{{ post.sitemap.priority }}< /priority >
      { % endif % }
    < /url >
  { % endfor % }
< /urlset >
```

#### 3.robots.txt 생성

- 1 ) github.io root 경로에 robots.txt 파일을 생성합니다.
- 2 ) 아래 내용을 robots.txt 파일에 작성합니다.
- 3 ) sitemap 에 자신의 블로그 주소를 넣어줍니다.

```html
User-agent: * Allow: / Sitemap: {{
'https://kyj0206.github.io/KYJ0206.Git_BLog/sitemap.xml' | relative_url |
prepend: site.url }}
```

#### 4.Google Search Console 에 sitemap 제출

- 1 ) Google Search Console에 접속합니다.
- 2 ) 본인의 github.io 속성을 선택하고, 왼쪽 메뉴에 색인 > Sitemaps 에 들어갑니다.
- 3 ) 새 사이트멥 추가에 sitemap.xml을 입력하고 제출합니다.

<a href="https://images.velog.io/images/kyj0206/post/fadec359-a01d-4ceb-ab50-60ae61326edd/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-28%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%2012.04.09.png">
![https://images.velog.io/images/kyj0206/post/fadec359-a01d-4ceb-ab50-60ae61326edd/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-28%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%2012.04.09.png](https://images.velog.io/images/kyj0206/post/fadec359-a01d-4ceb-ab50-60ae61326edd/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-28%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%2012.04.09.png)
</a>

- 4 ) 제출하고 2~3일 간 이후, sitemap 이 정상적으로 제출 되었는지 확인 해 줍니다.
  - 이후 제출 상태 성공이 적용되지 않는다면, URL 검사로 확인을 해 주세요.

<a href="https://images.velog.io/images/kyj0206/post/c46e4e9c-b49d-48bf-9333-6dd8a1759024/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.19.31.png">
![https://images.velog.io/images/kyj0206/post/c46e4e9c-b49d-48bf-9333-6dd8a1759024/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.19.31.png](https://images.velog.io/images/kyj0206/post/c46e4e9c-b49d-48bf-9333-6dd8a1759024/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202022-03-21%20%E1%84%8B%E1%85%A9%E1%84%92%E1%85%AE%201.19.31.png)
</a>

- 이후 사이트맵 제출이 정상적으로 진행이 되면, 아래와 같은 결과물을 보실 수 있습니다.<br/>

<a href="https://velog.velcdn.com/images/kyj0206/post/12c4c5ff-bb5c-4d75-b49f-fbf4bd915d6f/image.png">
![](https://velog.velcdn.com/images/kyj0206/post/12c4c5ff-bb5c-4d75-b49f-fbf4bd915d6f/image.png)
</a>

<br>

---

<br>

<span style='font-size:1rem'> **지금까지 Google SearchConsole에 대해 포스팅을 통해 배워 보았습니다.** </span><br>

<span style='font-size:1rem'> **애널리틱스와 더불어 서치콘솔을 이용하여,** </span><br>
<span style='font-size:1rem'> **앞으로 블로그를 더욱 편히 관리 해 보세요.** </span><br>

<span style='font-size:1rem'> **다음 포스팅은 더 유익한 정보로 찾아뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
