---
title: "[JavaScript] Scope(스코프)란?"
excerpt: "Scope란 무엇인지 알아보자"
categories:
  - JavaScript
tags:
  - [JavaScript, Scope]
toc: true
toc_sticky: true
published: true

date: 2025-02-12
last_modified_at: 2025-02-12
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 JavaScript Scope란**</span> <br>
<span style='font-size:1rem'>**무엇인지 자세히 알아 보겠습니다.**</span>

---

### [ JavaScript Scope란? ] <br>

<a href="/assets/images/Scope.png">
![/assets/images/Scope.png](/assets/images/Scope.png)
</a>

**스코프란** 단어의 뜻 그대로 **'범위'**라는 의미를 가지고있습니다.<br>
자바스크립트에서의 스코프는 **'변수에 접근할 수 있는 범위'**입니다.<br> <br>
자바스크립트에서 스코프는 크게 두가지 스코프로 나눌수 있습니다.

> **전역 스코프(Global Scope)**<br>
> 자바스크립트 전체 범위, 코드 어디에서든 참조가 가능한 스코프.

> **지역 스코프(Local Scope)**<br>
> 변수에 접근 또는 참조할 수 있는 범위가 함수 내부에만 정의되는 스코프.

#### JavaScript Scope 특징

- 자바스크립트의 스코프는 타 언어와는 다른 특징을 갖게 됩니다.
- C 기반 언어들은 블록 레벨 스코프(block-level scope) 를 따릅니다.
- 자바스크립트는 함수 레벨 스코프(Function-level scope) 를 따릅니다.
- 화살표 함수는 함수 스코프가 아니라 블록 스코프를 따릅니다.

##### 1. 블록 레벨 스코프(block-level scope)

- 코드블록 안에서 선언된 변수는 반드시 코드블록 안에서만 유효합니다.
- 코드의 오류등 이슈 가시성에 도움이 됩니다.

> ES6 이후에는 let, const가 추가 되면서 블록스코프를 선언할수 있습니다.

```javascript
var a = 1; // 전역 변수
console.log(a); // 1

{
  var a = 2; // 전역 변수
}

console.log(a); // 2
```

```javascript
let a = 1; // 전역 변수

{
  let a = 2; // 지역 변수
  let b = 2; // 지역 변수
}

console.log(a); // 1
console.log(b); // ReferenceError
```

##### 2. 함수 레벨 스코프(Function-level scope)

- 함수의 코드 블록만을 스코프로 범위 합니다.
- 내부에서 선언한 변수는 지역 변수가 되며 함수 외부에서 선언한 변수는 모두 전역 변수입니다.

> var 키워드로 선언한 변수들은 오로지 함수 스코프 만을 따릅니다.

```javascript
var test = test; // 전역 변수
function print() { // 지역(함수) 스코프
 var test = "Hello!"; // 지역 변수
 console.log(test); // Hello!
}
print();
console.log(test); // test
```

<br>

---

<br>

<span style='font-size:1rem'> **지금까지 JavaScript Scope에 대해 포스팅을 하였습니다.** </span><br>
<span style='font-size:1rem'> **도움이 되는 포스팅이었길 바랍니다.** </span><br>

<span style='font-size:1rem'> **감사합니다!** </span>