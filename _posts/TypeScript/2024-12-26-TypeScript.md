---
title: "[TypeScript] TypeScript란?"
excerpt: "TypeScript에 대해 알아보자"
categories:
  - TypeScript
tags:
  - [JavaScript,TypeScript]
toc: true
toc_sticky: true
published: true

date: 2024-12-26
last_modified_at: 2024-12-26
---

---

<span style='font-size:1rem'> **안녕하세요. Kim.YJ 입니다.** </span>

<span style='font-size:1rem'> **이번 포스팅은 마이크로소프트가 개발한 오픈소스 프로그래밍 언어로,** </span> <br>
<span style='font-size:1rem'> **타입스크립트(TypeScript)에 대해 알아보겠습니다.** </span>

---

### [ TypeScript 란? ] <br>

<a href="/assets/images/TypeScript.png">
![/assets/images/TypeScript.png](/assets/images/TypeScript.png)
</a>

**타입스크립트(TypeScript)는** 마이크로소프트가 개발한 오픈소스 프로그래밍 언어로, 자바스크립트의 상위 집합(Superset)입니다. <br><br>
자바스크립트의 모든 기능을 포함하며, 여기에 **정적 타입 검사**와 같은 기능을 추가하여 대규모 애플리케이션 개발을 더 안전하고 효율적으로 만들어줍니다. <br><br>
타입스크립트는 .ts 확장자를 사용하며, 자바스크립트로 컴파일되어 브라우저와 호환됩니다. 

---

### [ TypeScrip의 주요 특징 ]

TypeScrip는 다음과 같은 특징이 있습니다.

#### 1. **정적 타입 시스템**
- 변수와 함수에 타입을 명시할 수 있어, 컴파일 시점에 오류를 미리 확인할 수 있습니다.

```typescript
let age: number = 30;  // 정수형 변수
let name: string = "Kim";  // 문자열 변수
```

#### 2. **타입 추론**
- 타입스크립트는 코드에서 타입을 추론하여 명시적으로 선언하지 않아도 타입을 자동으로 결정합니다.

```typescript
let count = 10;  // number로 추론
```

#### 3. **인터페이스와 타입**
- 객체의 구조를 정의하고 코드의 일관성을 유지합니다.

```typescript
interface Person {
  name: string;
  age: number;
}
const kim: Person = { name: "Kim", age: 36 };
```

#### 4. **클래스와 객체지향 프로그래밍 지원**
- ES6+의 클래스 문법을 확장하며, 추상 클래스, 인터페이스, 접근 제한자(private, protected 등)를 지원합니다.

```typescript
class Animal {
  private name: string;

  constructor(name: string) {
    this.name = name;
  }

  move(distance: number): void {
    console.log(`${this.name} moved ${distance}m.`);
  }
}
```

#### 5. **강력한 도구 지원**
- Visual Studio Code 같은 에디터와 잘 통합되어 코드 자동완성, 오류 검사, 리팩토링 기능을 제공합니다.

#### 6. **모듈화 및 ES6+ 기능 지원**
- 최신 자바스크립트 기능을 사용할 수 있으며, 모듈 시스템(import/export)을 지원합니다.

---

### [ 타입스크립트를 사용하는 이유 ]

#### 1. **코드 품질 향상**
- 정적 타입 체크로 인해 런타임 오류가 줄어듭니다.

#### 2. **대규모 프로젝트 관리**
- 코드 가독성과 유지보수성이 높아집니다.

#### 3. **강력한 개발 도구 통합**
- IDE 지원으로 생산성이 향상됩니다.

#### 4. **점진적 도입 가능**
- 기존 자바스크립트 프로젝트에 타입스크립트를 부분적으로 도입할 수 있습니다.

---

### [ 타입스크립트 시작하기 ]

#### 1. **설치** 

```bash
npm install -g typescript
```

#### 2. **컴파일러 사용** 

```bash
tsc filename.ts
```

#### 3. **tsconfig.json 설정** 

```json
{
  "compilerOptions": {
    "target": "ES6",
    "module": "commonjs",
    "strict": true
  }
}
```

---

### [ 간단한 예제 ]

```typescript
function greet(user: { name: string; age: number }): string {
  return `안녕하세요, ${user.name} 입니다. 저의 나이는 ${user.age} 입니다.`;
}

const user = { name: "Youngjae", age: 36 };
console.log(greet(user)); // 안녕하세요, Kim.YJ 입니다. 저의 나이는 36 입니다.
```

<br>

---

<br>

<span style='font-size:1rem'> **지금까지 TypeScript에 대해 포스팅을 하였습니다.** </span><br>

<span style='font-size:1rem'> **도움이 되는 포스팅이었길 바랍니다.** </span><br>

<span style='font-size:1rem'> **감사합니다!** </span>