---
title: "[ React useEffect란 무엇인가? ]"
excerpt: "React useEffect란?"
categories:
  - React
tags:
  - [React, Hook, useEffect]
toc: true
toc_sticky: true
published: true

date: 2025-02-20
last_modified_at: 2025-02-20
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 React Hook - useEffect에 대해 포스팅 해 보겠습니다.**</span>

<span style='font-size:1rem'>**React useEffect에 대해 함께 알아 봅시다.**</span>

---

### [ React - useEffect란? ] <br>

<a href="/assets/images/useEffect.png">
![/assets/images/useEffect.png](/assets/images/useEffect.png)
</a>

useEffect()는 간단하게 말해 react component가 랜더링이 될때마다,<br>
sied effect를 실행할 수 있도록 하는 Hook입니다.<br>

component의 mount, unmount, update 에 따라,<br>
sied effect를 처리할 수 있습니다.

> sied effect - component의 랜더링 이후 비동기로 처리 되어야하는 효과

### [ useEffect - 사용방법 ] <br>
#### 1. 컴포넌트 마운트 시 한 번 실행 (빈 의존성 배열)
>	useEffect(() => {...}, []): 마운트 시 한 번만 실행

```react
import React, { useEffect } from 'react';

function ExampleComponent() {
  useEffect(() => {
    console.log('컴포넌트가 마운트되었습니다!');
  }, []); // 빈 배열 => 마운트 시 한 번만 실행

  return <div>Hello, React!</div>;
}
```

#### 2. 매 렌더링마다 실행 (의존성 배열 없음)
>	useEffect(() => {...}): 매 렌더링 시 실행

```react
import React, { useState, useEffect } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    console.log(`렌더링되었습니다. 현재 카운트: ${count}`);
  }); // 의존성 배열 없음 => 매 렌더링 시 실행

  return (
    <div>
      <p>카운트: {count}</p>
      <button onClick={() => setCount(count + 1)}>증가</button>
    </div>
  );
}
```

#### 3. 특정 상태 변경 시 실행 (의존성 배열 사용)
>	useEffect(() => {...}, [dep]): 특정 의존성 변경 시 실행

```react
import React, { useState, useEffect } from 'react';

function UserProfile({ userId }) {
  const [user, setUser] = useState(null);

  useEffect(() => {
    // userId가 변경될 때마다 API 호출
    fetch(`https://jsonplaceholder.typicode.com/users/${userId}`)
      .then((response) => response.json())
      .then((data) => setUser(data));
  }, [userId]); // userId 변경 시 실행

  if (!user) return <div>로딩 중...</div>;
  return <div>사용자 이름: {user.name}</div>;
}
```

#### 4. 클린업 함수 사용 (언마운트 시 실행)
>	useEffect(() => {... return () => {...} }, []): 마운트 시 실행 및 언마운트 시 클린업 수행

```react
import React, { useState, useEffect } from 'react';

function Timer() {
  const [seconds, setSeconds] = useState(0);

  useEffect(() => {
    const interval = setInterval(() => {
      setSeconds((prev) => prev + 1);
    }, 1000);

    // 클린업 함수: 언마운트 시 인터벌 해제
    return () => {
      clearInterval(interval);
      console.log('타이머가 정리되었습니다.');
    };
  }, []); // 마운트 시 실행 및 언마운트 시 정리

  return <div>타이머: {seconds}초</div>;
}
```

### [ useEffect 사용 시 주의사항 ] <br/>

useEffect는 React에서 비동기 작업, 구독,<br/>  
DOM 업데이트 등을 처리할 때 매우 유용하지만,<br/> 
잘못 사용하면 성능 저하나 버그를 유발할 수 있습니다. <br/>
다음은 주요 주의사항입니다.


| ⚡ **주의사항**                     | 📝 **설명**                                  |
|----------------------------------|----------------------------------|
| ✅ **의존성 배열 정확성**             | 모든 참조된 상태와 props를 배열에 포함해야 함       |
| 🧹 **클린업 함수 필수 사용**          | 타이머, 구독 해제 등 메모리 누수 방지              |
| ⚠️ **비동기 함수 처리 주의**          | `useEffect`에 직접 `async` 사용 금지            |
| 🔄 **불필요한 렌더링 방지**           | `useMemo`, `useCallback` 활용               |
| 🏃 **동기 작업 필요 시 `useLayoutEffect` 고려** | DOM 업데이트 직후 작업 처리            |

<br>
<br>
React useEffect란 간단하게 무엇인지<br>
간단한 사용 예시와 주의점을 알아 보았습니다.

<br>

---

<br>

<span style='font-size:1rem'> **지금까지 React useEffect에 대해 포스팅을 통해 알아 보았습니다.** </span><br>
<span style='font-size:1rem'> **다음 포스팅은 좀더 유용한 포스팅으로 찾아 뵙겠습니다.** </span><br>
<span style='font-size:1rem'> **감사합니다!** </span>
