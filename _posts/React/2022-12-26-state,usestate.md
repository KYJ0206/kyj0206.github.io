---
title: "[ State & useState ]"
excerpt: "State 와 useState 란?"
categories:
  - React
tags:
  - [React, State, useState, Hook]
toc: true
toc_sticky: true
published: true

date: 2022-12-26
last_modified_at: 2022-12-26
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 State,useState 에 대해 포스팅 해 보겠습니다.**</span>

<span style='font-size:1rem'>**State & useState 에 대해 함께 알아보고, 한 단계씩 배워 봅시다.**</span>

---

### [ ReactHook ] <br>

React Hook은 함수형 컴포넌트에 기능을 추가할 때 사용하는 함수다. 함수형 컴포넌트에서 상탯값을 사용할 수 있고 자식요소에 접근 할 수도있다.

### [ State 란? ] <br>

- state (상태) : 컴포넌트 내에서 동적으로 변경되는 값
- props는 (함수 매개변수처럼) 컴포넌트에 전달되는 반면, state는 (함수 내 선언된 변수처럼) 컴포넌트 안에서 관리된다는 차이가 있다.

> 쉽게 말해 state는 일반 변수와 다르게 값이 변하게 되면 렌더링이 일어난다. <br>
> 즉, 값이 변하게 되면 연관있는 컴포넌트들이 다시 렌더링이되어 화면이 바뀌게 된다. <br>
> state와 함께 사용되는 함수는 setState이다. <br>
> setState는 state 값을 변경시켜주는 함수이다.

```javascript
const [state, setState] = useState(초기값);
```

state는 위와 같이 선언한다. state는 변수, setState는 state를 변경시켜주는 함수, useState는 state, setState를 return 하면서 초기값을 설정해주는 hook이다.

state는 렌더링을 일으킬 수 있는 변수이다. setState는 state의 값을 변경할 때 사용하는 함수이다. useState는 state의 초기값을 정할 수 있고, return 값으로 state, setState를 돌려주는 hook이다.

### [ useState란? ] <br>

- useState는 컴포넌트에서 state값을 추가할때 사용된다. 함수형 컴포넌트에서는 클래스형 컴포넌트처럼 state를 사용할 수 없어, Hook을 사용해서 state와 같은 기능을 할 수 있도록 만들어주었다.

> 하나의 useState 함수는 하나의 상태 값만 관리를 할 수 있어 만약에 컴포넌트에서 관리해야 할 상태가 여러 개라면 useState 를 여러번 사용해야 한다.

사용법은 아래와 같습니다.

- import

```javascript
import React, { useState } from "react";
```

- useState 선언

```javascript
const [data, setData] = useState(0);
```

> data = state 값
>
> setData = data 값이 업데이트 되는 함수
>
> useState(0) = 첫 랜더링시 만 사용 되는 초기 state 설정값을 받는 인자

---

<span style='font-size:1rem'> **지금까지 State & useState 에 대해 포스팅을 통해 알아 보았습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
