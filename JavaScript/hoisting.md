# JavaScript Hoisting

Hoisting 이란? 인터프리터가 변수와 함수의 메모리 공간을 선언 전에 미리 할당하는 것을 의미한다.

1. `var` 로 선언시 `undefined` 로 변수를 초기화
2. `let` 과 `const`  호이스팅하되, 변수를 초기화하지 않는다.

[호이스팅 - 용어 사전 | MDN](https://developer.mozilla.org/ko/docs/Glossary/Hoisting)

## 호이스팅이 발생하는 이유

`JavaScript` 엔진에서 변수를 생성할때 어떤일이 일어지는지를 알면 이해하기 쉽다.

먼저 `JavaScript` 에서 변수는 1.선언 2.초기화 3.할당 순서로 이루어진다.
