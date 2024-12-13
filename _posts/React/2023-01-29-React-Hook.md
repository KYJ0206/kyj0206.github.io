---
title: "[ React Hook ]"
excerpt: "React Hook이란?"
categories:
  - React
tags:
  - [React, Hook]
toc: true
toc_sticky: true
published: true

date: 2023-01-29
last_modified_at: 2023-01-29
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 React Hook 에 대해 포스팅 해 보겠습니다.**</span>

<span style='font-size:1rem'>**React 에 대해 함께 알아보고, 한 단계씩 배워 봅시다.**</span>

---

### [ React Hook 이란? ] <br>

<a href="https://www.google.com/imgres?imgurl=https%3A%2F%2Fimages.velog.io%2Fimages%2Fkwonh%2Fpost%2Fbba244e8-1e64-49c9-85df-7bf4e4c0fdb3%2Fhook-logo.png&imgrefurl=https%3A%2F%2Fvelog.io%2F%40kwonh%2FReactHook-useState-%25EC%2599%2580-useEffect-%25EB%25A1%259C-%25EC%2583%2581%25ED%2583%25AF%25EA%25B0%2592%25EA%25B3%25BC-%25EC%2583%259D%25EB%25AA%2585%25EC%25A3%25BC%25EA%25B8%25B0-%25EC%2582%25AC%25EC%259A%25A9%25ED%2595%2598%25EA%25B8%25B0&tbnid=mVDQiVQ2C0UXqM&vet=12ahUKEwjdyLqYmuz8AhVHQN4KHZ9cB8UQMygCegUIARDDAQ..i&docid=UYZ6j_98yjkfTM&w=1166&h=926&q=%EB%A6%AC%EC%95%A1%ED%8A%B8%20%ED%9B%85&ved=2ahUKEwjdyLqYmuz8AhVHQN4KHZ9cB8UQMygCegUIARDDAQ">
![](https://velog.velcdn.com/images/kyj0206/post/40e37ed7-f9cc-447f-8530-c76e6b852e34/image.png)
</a>

이번 포스팅을 통해 Hook이란 무엇인지 간단하게 알아보는 시간을 가지겠습니다.

> Hook은 React 버전 16.8부터 React요소로 새로 추가되었습니다.
> Hook을 이용하여 기존 Class 바탕의 코드를 작성할 필요 없이 상태 값과 여러 React의 가능을 사용할 수 있습니다.
>
> -React 공식문서

리액트 hook은 React 16.8버전에 새로 추가된 기능으로, 함수형 컴포넌트에서 react state와 생명주기 기능(lifecycle features)을 "연동(hook into)할 수 있게 해준다. <br/><br/>
useState를 예시로 들면 class를 사용하지 않고도 상태를 가질 수 있게 된 것이다.<br/>
이전에 리액트가 겪던 문제들을 해결해주며 클래스형 컴포넌트를 사용하지 않고도<br/>
함수형 컴포넌트에서 상태값 접근과 자식 요소에 접근이 가능해졌다. <br/>
리액트는 useState, useEffect 같은 내장 Hook을 몇 가지 제공한다. <br/>
또한 props, state, context, refs 그리고 lifecycle과 같은 리액트 개념에 좀 더 직관적인 API를 제공한다. 또한 이 개념들을 엮기 위해 새로운 방법을 제공한다.
컴포넌트 간에 상태 관련 로직을 재사용하기 위해 hook을 직접 만드는 것도 가능하다.

### [ Hook의 장점 ] <br/>

> Hook 을 사용 했을때 장점을 확인 해 보겠습니다.

1. 컴포넌트로부터 상태 관련 로직을 추상화할 수 있다.<br/>
2. 이를 이용해 독립적인 재사용이 가능하다.<br/>
3. 코드의 재사용은 가독성을 높이고 유지보수를 용이하게 한다.<br/>
4. 훅은 계층의 변화 없이 상태 관련 로직을 재사용할 수 있다.<br/>
5. 생명주기 메서드를 기반으로 쪼개는 것 보다는 훅을 통해 작은 함수의 묶음으로 컴포넌트를 나누는 방법을 사용할 수 있다.

### [ React Hook의 필요성 ] <br>

> 함수 컴포넌트도 클래스 컴포넌트처럼 사용할 수 있다.
>
> 함수 컴포넌트는 클래스 컴포넌트와 다르게, 모듈로 활용하기가 쉽기 때문에
> 서로의 장점을 전부다 가지고 있다.

### [ React에서 기본적으로 지원하는 Hooks ]

> React 에서 기본으로 지원하는 Hooks 들을 알아 보겠습니다.
> 자세한 설명과 사용법은 각각의 포스팅을 통해 설명 하겠습니다.

1. **useState** - 컴포넌트의 state(상태)를 관리 할 수 있다.

2. **useEffect** - 렌더링 이후에 실행할 코드를 만들수 있다.

3. **useContext** - 부모컴포넌트와 자식컴포넌트 간의 변수와 함수를 전역적으로 정의할 수 있다.

4. **useReducer** - state(상태) 업데이트 로직을, reducer 함수에 따로 분리 할 수 있다.

5. **useRef** - 컴포넌트나 HTML 요소를 래퍼런스로 관리할 수 있다.

6. **forwardRef** - useRef로 만든 래퍼런스를 상위 컴포넌트로 전달할 수 있다.

7. **useImperativeHandle** - useRef로 만든 래퍼런스의 상태에 따라, 실행할 함수를 정의 할 수 있다.

8. **useMemo, useCallback** - 의존성 배열에 적힌 값이 변할 때만 값,함수를 다시 정의할 수 있다. ( 재랜더링시 정의 안함 )

9. **useLayoutEffect** - 모든 DOM 변경 후 브라우저가 화면을 그리기(render)전에 실행되는 기능을 정할 수 있다.

10. **useDebugValue** - 사용자 정의 Hook의 디버깅을 도와준다.

React 에서 기본으로 지원하는 Hooks와 간단한 설명을 리스트로 소개해 드렸습니다. <br/>
다음 포스팀을 통해 더 자세한 설명과 사용방법을 알려 드리겠습니다.

<br>

---

<br>

<span style='font-size:1rem'> **지금까지 React Hook에 대해 포스팅을 통해 알아 보았습니다.** </span><br>
<span style='font-size:1rem'> **다음 포스팅은 Hooks에 대한 더 자세한 정보로 찾아뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
