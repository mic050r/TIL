## 1. charCodeAt()

`charCodeAt()` 함수 : JavaScript 문자열에서 특정 위치의 문자에 해당하는 유니코드(Unicode) 코드 포인트를 반환하는 함수

→ 문자열 내의 각 문자는 유니코드 코드 포인트로 표현되며, 이 함수를 사용하면 해당 코드 포인트를 알 수 있음

`charCodeAt()` 함수의 기본 구문

```jsx
string.charCodeAt(index);
```

- `string`: 코드 포인트를 확인하려는 문자열
- `index`: 문자열 내에서 코드 포인트를 확인하려는 문자의 위치를 나타내는 인덱스. 0부터 시작하며, 음수 인덱스는 문자열의 끝에서부터 역순으로 접근.

`charCodeAt()` 함수는 문자열에서 지정된 위치의 문자의 유니코드 코드 포인트를 정수 형태로 반환→ 이 코드 포인트는 해당 문자의 고유한 숫자 식별자

ex) 영문 대문자 "A"의 유니코드 코드 포인트는 65이며, "B"는 66

예시 코드

```jsx
let str = "Hello, World!";
let firstChar = str.charCodeAt(0); // 'H'의 코드 포인트 (72)
let secondChar = str.charCodeAt(7); // ','의 코드 포인트 (44)
let exclamationPoint = str.charCodeAt(12); // '!'의 코드 포인트 (33)

console.log(firstChar); // 72
console.log(secondChar); // 44
console.log(exclamationPoint); // 33
```

`charCodeAt()` 함수는 유니코드 문자열을 다룰 때 유용하며, 문자열에서 문자의 위치 또는 코드 포인트를 확인할 때 활용할 수 있음.
