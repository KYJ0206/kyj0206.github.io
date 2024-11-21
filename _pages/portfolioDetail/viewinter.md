---
layout: single
title: "GENESISLAB VIEWINTER"
permalink: /portfolio/genesislab-viewinter/
toc: true
toc_sticky: true
published: true
description: "GENESISLAB VIEWINTER 프로젝트."
date: 2022-05-27
last_modified_at: 2022-05-27
---

## 📄 프로젝트 개요
<br/>
<a class="batimmage" href="/assets/images/Viewinter.png">
![/assets/images/Viewinter.png](/assets/images/Viewinter.png)
</a>

**GENESISLAB VIEWINTER HR**은 기업의 HR 데이터를 통합 관리하고 시각화하는 혁신적인 플랫폼입니다.  
인재 관리, 성과 평가, 근무 시간 추적 등 다양한 기능을 통해 조직의 효율성을 극대화하도록 설계되었습니다.

URL : <a href="https://viewinterhr.com/" target="_blank">GENESISLAB VIEWINTER HR</a>

---

### [기간] <br/>

2022.01 ~ 2022.05 ( 4개월 )

---

### [목표] <br/>

제네시스랩 Viewinter CMS 구축 개발

---

### [역할] <br/>

React 구조 설계 및 CSS 적용, HubL 개발 및 퍼블리셔

---

### [기여도] <br/>

내부 개발팀 총 2명 중 약 50% 기여 ( 퍼블리싱 파트 : 100% )

---

### [활동내용] <br/>

CMS 구축에 필요한 HubL 및 React를 사용 하여, 템플릿 및 구조 설계 및 개발 <br/> 
HubSpot API 연동 및 CSS 전반 퍼블리셔 업무 진행

---

### [주요기능]

기업의 HR 데이터를 관리하고 시각화하는 플랫폼으로, 인재 관리, 성과 평가, 근무 시간 추적 등의 기능을 제공합니다. <br/>
AI 채용 솔루션을 소개하며, 이 플랫폼은 기업 맞춤형 채용 및 인사 솔루션을 제공합니다. 

---

### [사용된기술] 

#### 1. **React**

- 컴포넌트 기반 개발: 재사용 가능한 컴포넌트를 통해 유지보수성과 확장성을 극대화. <br>
- 라우팅: React Router를 활용해 사용자 경험을 개선하는 동적 페이지 네비게이션 구현. <br>
- 퍼포먼스 최적화: 코드 스플리팅 및 Lazy Loading으로 초기 로딩 시간을 단축. <br>
- 스타일링 통합: CSS3와 함께 styled-components 또는 CSS Modules를 사용해 컴포넌트 단위의 유지보수성을 강화. <br>
- API 연동: React와 JavaScript의 Fetch API를 활용해 HubSpot 데이터와의 동적 연동 구현.

#### 2. **CSS3** (React 내 스타일링)

Flexbox, Grid, Slider 등 스타일링.

#### 3. **JavaScript** (React Context)

- 인터랙션 구현: 사용자 이벤트 핸들링 및 DOM 조작을 통해 대화형 인터페이스 구축.
- 상태 관리: React의 useState, useReducer와 Context API를 사용해 컴포넌트 간 데이터 공유.
- HubSpot 연동: React와 JavaScript로 HubL 데이터 바인딩 및 마케팅 자동화 처리.

#### 4. **HubL** (HubSpot Markup Language)

- HubSpot CMS에서의 데이터 바인딩과 템플릿 관리.
- 마케팅 자동화를 위한 동적 콘텐츠 생성에 사용.

#### 5. **HubSpot CMS**

- 템플릿 시스템을 통해 사이트 구조를 효율적으로 관리하고, 페이지 및 블로그 콘텐츠를 쉽게 업데이트 합니다.
- 모듈화된 콘텐츠 관리와 디자인 최적화를 통해 개발 속도와 유지 관리가 용이합니다.
- HubDB 사용 **DB (Database)** 관리 및 사용.

#### 6. **디자인 툴**

**Zeplin**: 디자이너와의 협업을 통해 UI/UX 프로토타입 제작. 

---

### [성과] <br/>

유지보수 1년 계약 

---

### [느낀점] 

#### 1. **React 첫 프로젝트** <br>

문제 설명 <br>
- React를 처음 사용한 프로젝트였기 때문에 컴포넌트 기반의 구조나 상태 관리에 대한 이해가 부족하여 코드의 유지보수성과 확장성에서 어려움이 있었습니다. 
- 특히, props와 state를 다루는 방식에 익숙하지 않아 코드 중복이 발생하고, 로직 구현이 복잡해졌습니다.

해결 방법 <br>
- React의 기본 개념인 컴포넌트화를 이해하고, 리팩토링을 통해 중복 코드를 제거했습니다.
- React의 상태 관리 방식을 명확히 이해하고, 각 컴포넌트의 책임을 분리하여 재사용 가능한 컴포넌트를 구현했습니다.
- 프로젝트 초기에는 작은 단위로 기능을 구현하고 점차적으로 확장하는 방식으로 진행하였습니다. 이를 통해 React의 컴포넌트 생명주기와 상태 관리에 대한 경험을 쌓을 수 있었습니다.


#### 2. **React 와 HubSpot 연동 문제** <br>

문제 설명 <br>
- HubSpot CMS에서 React 애플리케이션을 연동하는 과정에서 데이터 전달 및 동적 콘텐츠 생성 부분에서 어려움을 겪었습니다.
- HubSpot의 HubL(HubSpot Markup Language)과 React 간의 데이터 통신에 어려움이 있었고, 이를 해결하기 위해 API를 이용해야 했습니다.

해결 방법 <br>
- HubSpot API와 React를 연동하여 동적 콘텐츠를 처리하고, 필요한 데이터를 JSON 형식으로 받아 React 컴포넌트에서 렌더링할 수 있도록 했습니다.
- React의 Axios 라이브러리를 사용하여 API 요청을 처리하고, 데이터가 변경되면 자동으로 UI에 반영되는 방식으로 연동을 처리했습니다.
- HubSpot의 HubL 템플릿을 활용해 데이터를 미리 처리하고, React에서는 이를 동적으로 가져와 표시하는 방식으로 해결했습니다.

---