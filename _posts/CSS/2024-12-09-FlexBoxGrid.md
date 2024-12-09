---
title: "[CSS] FlexBox와 Grid"
excerpt: "CSS의 FlexBox와 Grid의 차이점"
categories:
  - CSS
tags:
  - [CSS, Layout]
toc: true
toc_sticky: true
published: true

date: 2024-12-09
last_modified_at: 2024-12-09
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 페이지에서 레이아웃을 구성할 때 자주 사용되는 CSS 속성 입니다. <br>
두 속성 모두 화면 요소를 배치하고 정렬하는 데에 사용되지만 몇가지 차이점이 존재합니다.** </span>

<span style='font-size:1rem'>**차이점과 특징을 자세히 알아 보겠습니다.**</span>

---

### [ 1차원 레이아웃 Flexbox ] 

#### 1. Flexbox의 특징

Flexbox는 1차원 레이아웃 속성으로, row 또는 column 중 하나를 기준으로 요소를 정렬하고 배치하는 데 최적화되어 있습니다.<br>
주로 행이나 열 중 하나의 방향으로 정렬해야 할 때 유용하며, 복잡한 행과 열을 모두 포함하는 레이아웃에서는 다소 한계가 있습니다.

#### 2. 사용 목적

Flexbox는 콘텐츠 중심으로, 콘텐츠가 추가되거나 줄어들 때 유연하게 대처하기 좋습니다. <br> 
예를 들어, 수평 또는 수직 방향으로 콘텐츠를 정렬하고 간격을 조절하는 데 유용하며, 버튼 그룹, 내비게이션 바 등 한 줄의 콘텐츠가 주가 되는 구성에 적합합니다.

#### 3. 기본 동작의 차이

Flexbox에서는 주로 요소가 컨테이너의 크기나 위치에 맞춰 자동으로 정렬됩니다. <br>  
Flexbox의 justify-content와 align-items 속성을 사용해, 주 축 방향으로 요소들을 배치하고 여백을 조절할 수 있습니다.

#### 4. FlexBox 사용방법

```css
display: Flex; // 컨테이너를 생성하기 위해 요소에 적용하는 속성입니다. 
flex-direction: Flex ; // 컨테이너 내에서 Flex 아이템들의 배치 방향을 지정하는 속성입니다. 
justify-content: Flex ; // 컨테이너 내에서 Flex 아이템들의 수평 방향 정렬 방법을 지정하는 속성입니다. 
align-items: Flex ; // 컨테이너 내에서 Flex 아이템들의 수직 방향 정렬 방법을 지정하는 속성입니다. 
flex-grow: Flex ; // 아이템이 Flex 컨테이너 내에서 차지하는 공간의 크기를 지정하는 속성입니다.
flex-shrink: Flex ; // 아이템이 Flex 컨테이너 내에서 차지하는 공간이 부족할 때, 아이템의 크기를 줄이는 정도를 지정하는 속성입니다.
flex-basis: Flex ; // 아이템의 초기 크기를 지정하는 속성입니다.
align-self: Flex ; // 컨테이너 내에서 개별 Flex 아이템의 수직 정렬 방법을 지정하는 속성입니다.
order: Flex ; // 컨테이너 내에서 Flex 아이템들의 순서를 지정하는 속성입니다.
```
<br> 

### [ 2차원 레이아웃 Grid ] 

#### 1. Grid의 특징

Grid는 2차원 레이아웃 속성으로, 행과 열을 모두 사용해 요소를 배치할 수 있습니다. <br> 
따라서 복잡한 레이아웃을 구성하거나, 웹페이지의 전체적인 구조를 잡는 데 적합합니다.

#### 2. 사용 목적

Grid는 레이아웃 중심으로 페이지 구조를 구성하는 데 최적화되어 있습니다. <br>  
예를 들어, 카드 레이아웃, 갤러리 형식 등 명확하게 구분된 영역을 기반으로 레이아웃을 구성할 때 Grid가 효과적입니다.

#### 3. 기본 동작의 차이

Grid는 행과 열을 사전에 정의하고 그 격자(grid cell)에 요소를 배치하는 방식입니다. <br> 
Grid에서는 grid-template-rows, grid-template-columns와 같은 속성으로 행과 열의 크기를 정의하고, 각 요소의 위치를 세밀하게 설정할 수 있습니다.

#### 4. Grid 사용방법

```css
display: Grid; // 컨테이너를 생성하기 위해 요소에 적용하는 속성입니다.
grid-template-columns, grid-template-rows: Grid; // 컨테이너 내에서 행과 열의 크기 및 개수를 지정하는 속성입니다.
grid-template-areas: Grid; // 컨테이너 내에서 그리드 영역의 이름을 지정하는 속성입니다.
grid-column-start, grid-column-end, grid-row-start, grid-row-end: Grid; //  아이템의 위치를 지정하는 속성입니다.
grid-area: Grid; // 아이템의 위치와 이름을 지정하는 속성입니다. 
grid-auto-rows, grid-auto-columns: Grid; // 컨테이너 내에서 자동으로 생성되는 행과 열의 크기를 지정하는 속성입니다.
grid-auto-flow: Grid; // 컨테이너 내에서 새로운 그리드 아이템이 생성될 때의 배치 방법을 지정하는 속성입니다.
justify-items, align-items: Grid; // 아이템들의 수평, 수직 정렬 방법을 지정하는 속성입니다.
justify-content, align-content: Grid; // 컨테이너 내에서 그리드 영역들의 수평, 수직 정렬 방법을 지정하는 속성입니다.
gap: Grid; // 아이템들과 그리드 영역 사이의 간격을 지정하는 속성입니다.
```

<br>

---

<span style='font-size:1rem'> **지금까지 CSS의 FlexBox와 Grid의 차이점에 대해 포스팅을 하였습니다.** </span><br>

<span style='font-size:1rem'> **도움이 되는 포스팅이었길 바랍니다.** </span><br>

<span style='font-size:1rem'> **다음 포스팅은 더 유익한 정보로 찾아뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
