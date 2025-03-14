---
title: "[ Pseudo-Elements/Class ]란 무엇인가요?"
excerpt: "의사요소와 의사클래스에 대해 알아보자"
categories:
  - CSS
tags:
  - [Pseudo-Elements, Pseudo-Class]
toc: true
toc_sticky: true
published: true

date: 2025-03-14
last_modified_at: 2025-03-14
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 CSS에서 유용하게 사용하는,**</span> <br>
<span style='font-size:1rem'>**의사 요소와 의사 클래스에 대해,**</span> <br>
<span style='font-size:1rem'>**알아 보겠습니다.**</span>

<span style='font-size:1rem'>**지금부터 자세히 설명 드릴테니,**</span> <br>
<span style='font-size:1rem'>**천천히 이해하며 진행해 주시면 감사하겠습니다.**</span>

---

### [ 의사 요소(pseudo-element) 란? ] <br>

의사 요소(pseudo-element)는 해당 HTML 요소의 특정 부분만을 선택할 때 사용합니다.

#### 문법<br>
선택자::의사요소이름 {속성: 속성값;}

#### 대표적인 요소<br>

| 선택자        | 설명 |
|--------------|--------------------------|
| `::first-letter` | 텍스트의 첫 글자만 선택. |
| `::first-line`   | 텍스트의 첫 라인만 선택. |
| `::before`       | 특정 요소의 바로 앞에 요소 삽입. |
| `::after`        | 특정 요소의 바로 뒤에 요소 삽입. |
| `::selection`    | 사용자가 선택한 부분만 선택. |

#### 예제<br>
```css
<style>
    p::first-letter { color: red;}
</style>
```

### [ 의사 클래스(pseudo-class) 란? ] <br>

CSS에서 의사 클래스(pseudo-class)는 선택하고자 하는 HTML 요소의 특별한 '상태(state)'를 명시할 때 사용합니다.

#### 문법<br>
선택자:의사클래스이름 {속성: 속성값;} 

#### 대표적인 요소<br>

| 선택자        | 설명 |
|--------------|--------------------------|
| `:link` | 페이지를 방문하지 않은 상태를 모두 선택. |
| `:visited`   | 링크를 통해서 연결된 페이지를 방문한 상태 선택. |
| `:hover`       | 마우스 커서가 링크 위에 올라가 있는 상태 선택. |
| `:active`        | 클릭하고 있는 상태를 모두 선택함. |
| `:focus`    | 초점이 맞춰진 input 요소를 모두 선택함. |
| `:checked`    | 체크된(checked) 상태의 input 요소를 모두 선택. |
| `:enabled`    | 사용할 수 있는 input 요소를 모두 선택. |
| `:disabled`    | 사용할 수 없는 input 요소를 모두 선택. |
| `:target`    | 활성화된 target 요소를 모두 선택. |
| `:in-range`    | 특정 범위 내의 값을 가지는 input 요소를 모두 선택. |
| `:out-of-range`    | 특정 범위를 벗어나는 값을 가지는 input 요소를 모두 선택. |
| `:read-only`    | readonly 속성을 가지는 input 요소를 모두 선택. |
| `:read-write`    | readonly 속성을 가지지 않는 input 요소를 모두 선택. |
| `:required`    | 	required 속성을 가지는 input 요소를 모두 선택. |
| `:optional`    | required 속성을 가지지 않는 input 요소를 모두 선택. |
| `:valid`    | 유효한 값을 가지는 input 요소를 모두 선택. |
| `:invalid`    | 	유효하지 않은 값을 가지는 input 요소를 모두 선택. |
| `:first-child`    | 요소 중에서 첫 번째에 위치하는 자식(child) 요소를 모두 선택. |
| `:last-child`    | 요소 중에서 마지막에 위치하는 자식(child) 요소를 모두 선택. |
| `:nth-child`    | 요소 중에서 앞에서부터 n번째에 위치하는 자식(child) 요소를 모두 선택. |
| `:nth-last-child`    | 요소 중에서 뒤에서부터 n번째에 위치하는 자식(child) 요소를 모두 선택. |
| `:first-of-type`    | 요소 중에서 첫 번째로 등장하는 특정 요소를 모두 선택. |
| `:last-of-type`    | 요소 중에서 마지막으로 등장하는 특정 요소를 모두 선택. |
| `:nth-of-type`    | 요소 중에서 n번째로 등장하는 특정 요소를 모두 선택. |
| `:nth-last-of-type`    | 요소 중에서 뒤에서부터 n번째로 등장하는 특정 요소를 모두 선택. |
| `:only-child`    | 요소를 단 하나만 가지는 모든 요소의 자식(child) 요소를 선택. |
| `:only-of-type`    | 특정 요소 단 하나만 가지는 모든 요소의 자식(child) 요소를 선택. |
| `:empty`    | 아무런 자식(child) 요소도 가지지 않는 요소를 모두 선택. |
| `:root`    | 문서의 root 요소를 선택. |
| `:not`    | 모든 선택자와 함께 사용할 수 있으며, 해당 선택자를 반대로 적용. |
| `:lang`    | 특정 요소를 언어 설정에 따라 다르게 표현할 때에 사용. |

#### 예제<br>
```css
<style>
    p:hover { border: 1px solid #000;}
</style>
```


### [ 의사 요소와 의사 클래스의 차이점 ] <br>

의사 요소는 요소의 특정 부분에 스타일을 적용하는 반면, <br>
의사클래스는 요소의 상태나 조건을 기반으로 스타일을 변경한다는 점에서 차이가 있습니다.<br><br>

의사 클래스는 "상태/조건"을 기준으로 동작하고, 의사요소는 "특정부분"을 기준으로 동작한다고 이해하면 됩니다.

<br>

---

<br>

<span style='font-size:1rem'> **의사 요소와 의사 클래스에 대해 포스팅을 하였습니다.** </span><br>

<span style='font-size:1rem'> **도움이 되는 포스팅이었길 바랍니다.** </span><br>

<span style='font-size:1rem'> **다음 포스팅은 더 유익한 정보로 찾아뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
