# **String.fromCharCode()**

`String.fromCharCode()` 함수 : JavaScript에서 사용되며, 하나 이상의 유니코드 코드 포인트를 가지고 문자열을 생성하는 데 사용

→ 유니코드 코드 포인트를 문자열로 변환하는 역할

`String.fromCharCode()` 함수의 구문

```jsx
String.fromCharCode(codePoint1[, codePoint2[, ...[, codePointN]]])

```

- `codePoint1`, `codePoint2`, ... `codePointN`: 생성하려는 문자열의 각 문자에 해당하는 유니코드 코드 포인트. 여러 개의 코드 포인트를 인수로 전달할 수 있으며, 이들은 문자열에 순서대로 결합됨

예시 코드

```jsx
let str = String.fromCharCode(72, 101, 108, 108, 111);
console.log(str); // "Hello"

```

위의 예시에서 `String.fromCharCode()` 함수는 유니코드 코드 포인트 72에 해당하는 문자 "H", 101에 해당하는 문자 "e", 108에 해당하는 문자 "l"을 차례로 결합하여 문자열 "Hello"를 생성.

이 함수는 주로 유니코드 코드 포인트를 문자열로 변환할 때 사용됨