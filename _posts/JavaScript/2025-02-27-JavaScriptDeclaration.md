---
title: "[JavaScript] var,let,const란?"
excerpt: "자바스크립트의 var,let,const가 무엇인지 알아보자"
categories:
  - JavaScript
tags:
  - [JavaScript, Declaration]
toc: true
toc_sticky: true
published: true

date: 2025-02-27
last_modified_at: 2025-02-27
---

---

<span style='font-size:1rem'>**안녕하세요. Kim.YJ 입니다.**</span>

<span style='font-size:1rem'>**이번 포스팅은 JavaScript Scope에 이어**</span> <br>
<span style='font-size:1rem'>**자바스크립트의 변수 선언방식 var,let,const란**</span> <br>
<span style='font-size:1rem'>**무엇인지 자세히 알아 보겠습니다.**</span>

---

### [ JavaScript Declaration란? ] <br>

<a href="/assets/images/jsVariables.png">
![/assets/images/jsVariables.png](/assets/images/jsVariables.png)
</a>

**선언** 단어의 뜻 그대로 **'변수를 만드는 과정'**이라는 의미를 가지고있습니다.<br>
자바스크립트에서의 변수는 선언과 할당을 통해 사용할수 있습니다.<br> <br>
자바스크립트에서 변수 선언 방식은 세가지 방식으로 나눌수 있습니다.<br>
ES6 이전에는 **var**가 유일한 변수 선언 방식이어서 사용을 하였지만,<br>
ES6 이후 **let**과 **const** 선언식의 등장으로 코드중복 오류의 가능성이나,<br>
가독성 및 유지보수등의 이유로 최신 자바스크립트에서는 **let**과 **const**를 선호합니다.

####  **var(function-level scope)**

> 선언된 함수내부 어디에서든 참조가 가능한 스코프 입니다.<br>
> 중복선언과 재할당이 모두 가능합니다.<br>
> 최종변수의 값은 마지막에 할당된 값입니다.<br>

```javascript
var name = kim; 
console.log(name); // kim

var name = kim.YJ;
console.log(name); // kim.YJ

name = who is;
console.log(name); // who is (마지막 할당된 값)
```

#### **let(block-level scope)**

> 블록{} 내부에서만 참조됩니다.<br>
> 중복선언과 불가능합니다.<br>
> 재할당은 가능합니다.<br>

```javascript
let name = kim; 
let name = kim.YJ;
cnosole.log(name); // 중복선언을 허용하지 않아 SyntaxError 발생
```

```javascript
let name = kim; 
cnosole.log(name); // kim

name = kim.YJ;
cnosole.log(name); // kim.YJ
```

#### **const(block-level scope)**

> **const(block-level scope)**<br>
> 블록{} 내부에서만 참조됩니다.<br>
> 중복선언과 불가능합니다.<br>
> 상수를 선언하는 키워드이기에 재할당 또한 불가능 합니다.<br>

```javascript
const name = kim;
const name = kim.YJ;
cnosole.log(name); // 중복선언을 허용하지 않아 SyntaxError 발생
```

```javascript
const name = kim;
cnosole.log(name); // kim

name = kim.YJ;
cnosole.log(name); // 재할당을 허용하지 않아 SyntaxError 발생
```

<br>

---

<br>

<span style='font-size:1rem'> **지금까지 JavaScript 변수선언식에 대해 포스팅을 하였습니다.** </span><br>
<span style='font-size:1rem'> **도움이 되는 포스팅이었길 바랍니다.** </span><br>

<span style='font-size:1rem'> **감사합니다!** </span>