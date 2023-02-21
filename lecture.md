# 목차
- [목차](#목차)
- [1. HTML/CSS 기초](#1-htmlcss-기초)
  - [1.1. HTML 기초: 문서 구조, 태그, 속성, 요소 등](#11-html-기초-문서-구조-태그-속성-요소-등)
  - [1.2. CSS 기초: 선택자, 속성, 값, 박스 모델 등](#12-css-기초-선택자-속성-값-박스-모델-등)
  - [1.3. HTML과 CSS를 사용하여 간단한 웹 페이지 작성](#13-html과-css를-사용하여-간단한-웹-페이지-작성)
- [2. JavaScript 기초](#2-javascript-기초)
  - [2.1. 변수, 데이터 타입, 연산자, 조건문, 반복문 등](#21-변수-데이터-타입-연산자-조건문-반복문-등)
  - [2.2. 비동기처리(async, await, promise)](#22-비동기처리async-await-promise)
  - [2.3. 함수, 객체, 배열 등](#23-함수-객체-배열-등)
  - [2.4. DOM(Document Object Model) 이해 및 조작](#24-domdocument-object-model-이해-및-조작)
  - [2.5. 배열함수 및 lodash.js, moment.js](#25-배열함수-및-lodashjs-momentjs)
- [3. SAPUI5 프레임워크](#3-sapui5-프레임워크)
  - [3.1. SAPUI5 소개와 설치](#31-sapui5-소개와-설치)
  - [3.2. 모델, 뷰, 컨트롤러(MVC) 패턴](#32-모델-뷰-컨트롤러mvc-패턴)
    - [3.2.1. Model](#321-model)
    - [3.2.2. View](#322-view)
    - [3.2.3. Controller](#323-controller)
  - [3.3. SAPUI5 컨트롤러 종류와 사용 방법](#33-sapui5-컨트롤러-종류와-사용-방법)
    - [3.3.1. XML 뷰 컨트롤러](#331-xml-뷰-컨트롤러)
    - [3.3.2. JavaScript 뷰 컨트롤러](#332-javascript-뷰-컨트롤러)
    - [3.3.3. JSON 모델 컨트롤러](#333-json-모델-컨트롤러)
  - [3.4. SAPUI5 라우팅 및 네비게이션](#34-sapui5-라우팅-및-네비게이션)
    - [라우팅 구성요소](#라우팅-구성요소)
  - [3.5. SAPUI5 데이터 바인딩과 포맷팅](#35-sapui5-데이터-바인딩과-포맷팅)
  - [3.6. SAPUI5 이벤트 처리와 메시지 관리](#36-sapui5-이벤트-처리와-메시지-관리)
  - [3.7. SAPUI5 국제화 및 로컬라이제이션](#37-sapui5-국제화-및-로컬라이제이션)
  - [3.8. SAPUI5 디버깅 및 테스팅](#38-sapui5-디버깅-및-테스팅)
- [4. 추가 학습 사항](#4-추가-학습-사항)
  - [4.1. OData와의 연동](#41-odata와의-연동)
  - [4.2. SAP Fiori 디자인 지침](#42-sap-fiori-디자인-지침)
  - [4.3. SAPUI5 응용프로그램의 배포와 유지보수](#43-sapui5-응용프로그램의-배포와-유지보수)

# 1. HTML/CSS 기초
 ## 1.1. HTML 기초: 문서 구조, 태그, 속성, 요소 등
```html
<!DOCTYPE html>
<html>
  <head>
    <title>문서 제목</title>
    <!-- 스타일 시트와 스크립트를 링크하는 태그 등을 포함합니다. -->
  </head>
  <body>
    <!-- 웹 페이지의 내용을 구성하는 태그들을 포함합니다. -->
  </body>
</html>
```
## 1.2. CSS 기초: 선택자, 속성, 값, 박스 모델 등
 > **Element Selector**  : HTML 요소의 태그명으로 지정
```css
div { color: red; }
p { color: red; }
```
 > **Class Selector**  : HTML 요소의 class 속성으로 지정
```css
.class-name { color: red; }
```
 > **ID Selector**  : HTML 요소의 id 속성으로 지정
```css
#id-name { color: red; }
```
 > **Attribute Selector**  : HTML 요소의 속성으로 지정
```css
[type="text"] { color: red; }
[data-type="text"] { color: red; }
```
 > **Child Selector**  : HTML 요소의 하위 요소 중 특정 요소를 선택
```css
div > p { color: red; }
```
 > **주요 속성**
 ```css
div {
    width: 200px;
    height: 200px;
    padding: 10px;
    border: 1px solid black;
    margin: 10px;
}
.text {
    font-family: "Helvetica Neue", sans-serif;  // 글꼴 지정
    font-size: 16px; // 글꼴 크기
    font-weight: bold; // 글꼴 두께
    font-style: italic; // 글꼴 스타일
    line-height: 1.5; // 텍스트 라인 간의 간격
    letter-spacing: 2px; // 글자 간 간격
    word-spacing: 5px; // 단어 간 간격
}
```
 > **Flex Box**
* https://blog.webdevsimplified.com/2021-11/flexbox/
 > **CSSGrid**
* https://blog.logrocket.com/css-grid-guide/****
## 1.3. HTML과 CSS를 사용하여 간단한 웹 페이지 작성
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My First Web Page</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header>
      <h1>My First Web Page</h1>
    </header>

    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>

    <section>
      <h2>About Me</h2>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis efficitur
        magna vel ipsum suscipit pharetra. In hac habitasse platea dictumst.
        Maecenas congue neque et efficitur commodo. Praesent bibendum velit
        lectus, vel fringilla dolor consectetur ac. Sed in lacinia risus.
      </p>
    </section>

    <footer>
      <p>&copy; 2023 My First Web Page</p>
    </footer>
  </body>
</html>
```
```css
body {
  font-family: Arial, sans-serif;
  background-color: #f8f8f8;
}

header {
  background-color: #333;
  color: #fff;
  padding: 20px;
}

nav {
  background-color: #666;
  color: #fff;
  padding: 10px;
}

nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
}

nav ul li {
  margin-right: 20px;
}

nav ul li a {
  color: #fff;
  text-decoration: none;
}

section {
  padding: 20px;
}

footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  padding: 10px;
}
```
---

<br />

# 2. JavaScript 기초
## 2.1. 변수, 데이터 타입, 연산자, 조건문, 반복문 등
```js
// 변수 선언
let x = 10;
const y = 20;

// 데이터 타입
const a = true;
const b = 1;
const c = "Hello";
const d = null;
const e = undefined;
const f = Symbol();
const g = {};
const h = function() {};
const i = new Map();
const j = new Set();

// 산술 연산자
const sum = x + y;
const diff = x - y;
const product = x * y;
const quotient = x / y;
const remainder = x % y;

// 비교 연산자
const isEqual = x === y;
const isNotEqual = x !== y;
const isGreaterThan = x > y;
const isLessThan = x < y;

// 논리 연산자
const andResult = a && b;
const orResult = a || b;
const notResult = !a;

// 대입 연산자
let z = 5;
z += 1;
z -= 1;
z *= 2;
z /= 2;

// 조건문
if (x > y) {
  console.log("x is greater than y");
} else {
  console.log("y is greater than or equal to x");
}

switch (x) {
  case 0:
    console.log("x is 0");
    break;
  case 1:
    console.log("x is 1");
    break;
  default:
    console.log("x is neither 0 nor 1");
    break;
}

// 반복문
for (let i = 0; i < 10; i++) {
  console.log(i);
}

let i = 0;
while (i < 10) {
  console.log(i);
  i++;
}

do {
  console.log(i);
  i++;
} while (i < 10);

// arrow function
const add = (a, b) => a + b;
const multiply = (a, b) => {
  return a * b;
};

// spread operator
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const mergedArr = [...arr1, ...arr2];

const obj1 = { x: 1, y: 2 };
const obj2 = { z: 3 };
const mergedObj = { ...obj1, ...obj2 };

function sum(a, b, c) {
  return a + b + c;
}
const arr = [1, 2, 3];
const result = sum(...arr);

// rest parameter
function average(...args) {
  const sum = args.reduce((acc, curr) => acc + curr, 0);
  return sum / args.length;
}
const avg = average(1, 2, 3, 4, 5);
```
## 2.2. 비동기처리(async, await, promise)
* [Deeply Understanding JavaScript Async and Await with Examples](https://blog.bitsrc.io/understanding-javascript-async-and-await-with-examples-a010b03926ea)
* [자바스크립트 Promise 쉽게 이해하기](https://joshua1988.github.io/web-development/javascript/promise-for-beginners/)
* [Understanding Promise.all in JavaScript](https://blog.logrocket.com/understanding-promise-all-in-javascript/)
## 2.3. 함수, 객체, 배열 등
> 함수
```javascript
function functionName(parameter1, parameter2, ...) {
  // 함수 내부에서 수행할 작업
  return result;
}
```
> 객체
```javascript
let objectName = {
  propertyName1: value1,
  propertyName2: value2,
  ...
}
```
> 배열
```javascript
let arrayName = [element1, element2, ...];
```
## 2.4. DOM(Document Object Model) 이해 및 조작
```javascript
document.getElementById(id)
document.getElementsByClassName(className)
document.getElementsByTagName(tagName)
document.querySelector(selector)
document.querySelectorAll(selector)
```
## 2.5. 배열함수 및 lodash.js, moment.js
* [lodash.js](https://lodash.com/docs/4.17.15)
* [moment.js](https://momentjs.com/docs/)
* 배열함수
> push() - 배열의 끝에 하나 이상의 요소를 추가
```javascript
const arr = [1, 2, 3];
arr.push(4);
console.log(arr); // [1, 2, 3, 4]
```
> pop() - 배열의 마지막 요소를 제거
```javascript
const arr = [1, 2, 3];
arr.pop();
console.log(arr); // [1, 2]
```
> shift() - 배열의 첫 번째 요소를 제거하고, 나머지 요소를 앞으로 이동
```javascript
const arr = [1, 2, 3];
arr.shift();
console.log(arr); // [2, 3]
```
> unshift() - 배열의 맨 앞에 하나 이상의 요소를 추가
```javascript
const arr = [1, 2, 3];
arr.unshift(0);
console.log(arr); // [0, 1, 2, 3]
```
> splice() - 배열의 중간에 하나 이상의 요소를 추가하거나 제거
```javascript
const arr = [1, 2, 3, 4, 5];
arr.splice(2, 1); // 인덱스 2부터 1개의 요소를 제거
console.log(arr); // [1, 2, 4, 5]

arr.splice(2, 0, 'a', 'b'); // 인덱스 2에 'a', 'b' 추가
console.log(arr); // [1, 2, 'a', 'b', 4, 5]
```
> concat() - 배열을 병합하여 새로운 배열을 반환
```javascript
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const newArr = arr1.concat(arr2);
console.log(newArr); // [1, 2, 3, 4, 5, 6]
```
> slice() - 배열의 일부분을 선택하여 새로운 배열을 반환
```javascript
const arr = [1, 2, 3, 4, 5];
const newArr = arr.slice(2, 4);
console.log(newArr); // [3, 4]
```
> sort() - 배열의 요소를 정렬
```javascript
const arr = [5, 2, 4, 1, 3];
arr.sort();
console.log(arr); // [1, 2, 3, 4, 5]
```
> reverse() - 배열의 요소를 역순으로 정렬
```javascript
const arr = [1, 2, 3];
arr.reverse();
console.log(arr); // [3, 2, 1]
```
> Array.find() - 주어진 판별 함수를 만족하는 첫 번째 요소의 값을 반환
```javascript
const arr = [1, 2, 3, 4, 5];
const result = arr.find((value) => value > 2);
console.log(result); // 3
```
> Array.findIndex() - Array.find() 함수와 유사하게 동작하지만, 판별 함수를 만족하는 첫 번째 요소의 인덱스를 반환
```javascript
const arr = [1, 2, 3, 4, 5];
const result = arr.findIndex((value) => value > 2);
console.log(result); // 2
```
> Array.forEach() - 배열의 각 요소에 대해 인자로 주어진 함수를 실행
```javascript
const arr = [1, 2, 3, 4, 5];

arr.forEach((value, index, array) => {
  console.log(`Value: ${value}, Index: ${index}, Array: ${array}`);
  // Value: 1, Index: 0, Array: [1, 2, 3, 4, 5]
  // Value: 2, Index: 1, Array: [1, 2, 3, 4, 5]
  // Value: 3, Index: 2, Array: [1, 2, 3, 4, 5]
  // Value: 4, Index: 3, Array: [1, 2, 3, 4, 5]
  // Value: 5, Index: 4, Array: [1, 2, 3, 4, 5]
});
```
> Array.map() - 배열의 각 요소에 대해 인자로 주어진 함수를 실행한 결과를 새로운 배열로 반환
```javascript
const arr = [1, 2, 3, 4, 5];

const newArr = arr.map((value, index, array) => {
  return value * 2;
});

console.log(newArr); // [2, 4, 6, 8, 10]
```
> Array.filter() - 배열의 각 요소에 대해 인자로 주어진 함수를 실행한 결과가 true인 요소들로 이루어진 새로운 배열을 반환
```javascript
const arr = [1, 2, 3, 4, 5];

const filteredArr = arr.filter((value, index, array) => {
  return value % 2 === 0;
});

console.log(filteredArr); // [2, 4]
```
> Array.reduce() - 배열의 각 요소에 대해 인자로 주어진 함수를 실행하여 하나의 결과값을 반환
```javascript
const arr = [1, 2, 3, 4, 5];

const sum = arr.reduce((accumulator, currentValue, index, array) => {
  return accumulator + currentValue;
});

console.log(sum); // 15
```
> Array.every() - 배열의 모든 요소에 대해 인자로 주어진 함수를 실행하여 결과가 모두 true인지 아닌지를 반환
```javascript
const arr = [1, 2, 3, 4, 5];

const isPositive = arr.every((value, index, array) => {
  return value > 0;
});

console.log(isPositive); // true
```
> Array.some() - 배열의 일부 요소에 대해 인자로 주어진 함수를 실행하여 결과가 하나 이상 true인지 아닌지를 반환
```javascript
const arr = [1, -2, 3, -4, 5];

const hasNegative = arr.some((value, index, array) => {
  return value < 
```
---
# 3. SAPUI5 프레임워크
## 3.1. SAPUI5 소개와 설치
> * SAPUI5는 SAP에서 개발한 오픈 소스 웹 프레임워크로, 모바일과 데스크톱에서 사용 가능한 반응형 웹 어플리케이션을 쉽게 개발할 수 있도록 도와줍니다. SAPUI5는 HTML5, CSS3, JavaScript, jQuery 등을 기반으로 하며, MVC(Model-View-Controller) 디자인 패턴을 사용하여 개발을 진행합니다.
> * SAPUI5를 사용하려면, JavaScript와 jQuery 등의 지식이 필요합니다. 또한 SAPUI5는 OData(Organization for the Advancement of Structured Information Standards)를 기반으로 하는 SAP Gateway와 연동하여 데이터를 처리합니다. 따라서 SAP Gateway를 사용하기 위해서는 OData에 대한 이해가 필요합니다.
## 3.2. 모델, 뷰, 컨트롤러(MVC) 패턴
### 3.2.1. Model
> * SAPUI5에서는 데이터 모델링을 위해 JSON, XML, OData 등 다양한 형태의 데이터 모델을 지원합니다.
> * 데이터 모델을 만들고 사용하기 위해서는 sap.ui.model 패키지에서 제공하는 클래스들을 사용합니다.

### 3.2.2. View
> * SAPUI5에서는 XML, HTML, JavaScript 등을 사용하여 UI를 구성할 수 있습니다.
> * View를 만들기 위해서는 sap.ui.core.mvc 패키지에서 제공하는 sap.ui.core.mvc.View 클래스를 상속받아 사용합니다.

### 3.2.3. Controller
> * SAPUI5에서는 Controller를 사용하여 애플리케이션의 로직을 처리합니다.
> * Controller를 만들기 위해서는 sap.ui.core.mvc 패키지에서 제공하는 sap.ui.core.mvc.Controller 클래스를 상속받아 사용합니다.
## 3.3. SAPUI5 컨트롤러 종류와 사용 방법
### 3.3.1. XML 뷰 컨트롤러
> XML 뷰 파일에 선언된 컨트롤러입니다. XML 뷰 파일의 "controllerName" 속성에 컨트롤러 클래스 이름을 지정하여 해당 컨트롤러와 XML 뷰를 연결합니다. 컨트롤러 클래스에는 이벤트 처리기 및 뷰와 관련된 로직이 포함됩니다.
### 3.3.2. JavaScript 뷰 컨트롤러
> JavaScript 파일에 직접 구현된 컨트롤러입니다. XML 뷰와 마찬가지로, "controllerName" 속성에 컨트롤러 클래스 이름을 지정하여 해당 컨트롤러와 뷰를 연결합니다. 컨트롤러 클래스에는 이벤트 처리기 및 뷰와 관련된 로직이 포함됩니다.
### 3.3.3. JSON 모델 컨트롤러
>JSON 파일로부터 데이터를 로드하고 뷰에 데이터를 바인딩하는 데 사용됩니다. 컨트롤러 클래스에는 데이터 로드 및 처리 로직이 포함됩니다.
## 3.4. SAPUI5 라우팅 및 네비게이션
[Documentation](https://sapui5.hana.ondemand.com/sdk/#/topic/3d18f20bd2294228acb6910d8e8a5fb5)
> 라우팅은 URL을 기반으로 사용자가 요청한 페이지를 동적으로 생성하는 기술입니다. 이를 통해 SPA(Single Page Application)를 구현할 수 있습니다.
> * SAPUI5에서 라우팅을 구현하기 위해서는 'sap.ui.core.routing.Router' 클래스를 사용합니다. 이 클래스는 라우팅 정보를 정의하고, URL과 뷰 간의 매핑을 수행합니다. 'sap.ui.core.routing.Route' 클래스는 개별 라우팅을 정의하는 데 사용됩니다.
> * 라우팅 정보를 정의한 후, initialize() 메서드를 호출하여 라우터를 초기화합니다. 이 때, sap.ui.core.UIComponent 클래스에서는 init() 메서드 내부에서 initialize() 메서드를 호출합니다.
> * 라우터를 초기화한 후, navTo() 메서드를 호출하여 라우팅을 수행합니다. 이 메서드는 라우팅 이름과 라우팅 매개변수를 인자로 받습니다. 라우팅 매개변수는 URL 패턴 내에 존재하는 변수 값입니다.
### 라우팅 구성요소
> * name: 라우팅 이름
> * pattern: URL 패턴
> * target: 라우팅 대상 뷰
> * viewType: 뷰 타입(XML, JSON, JS 등)
> * viewPath: 뷰가 위치한 경로
> * viewName: 뷰 이름
> * callback: 라우팅이 활성화될 때 실행할 콜백 함수
## 3.5. SAPUI5 데이터 바인딩과 포맷팅
## 3.6. SAPUI5 이벤트 처리와 메시지 관리
## 3.7. SAPUI5 국제화 및 로컬라이제이션
## 3.8. SAPUI5 디버깅 및 테스팅
---****
# 4. 추가 학습 사항
## 4.1. OData와의 연동
## 4.2. SAP Fiori 디자인 지침
## 4.3. SAPUI5 응용프로그램의 배포와 유지보수