# **Array.from()**

`Array.from()` 함수는 JavaScript에서 사용되는 배열을 생성하고, 유사 배열 객체나 이터러블 객체(예: 문자열, Set, Map 등)를 배열로 변환하는 메서드

기본 형식

```jsx
Array.from(arrayLike[, mapFn[, thisArg]])

```

1. `arrayLike`: 배열로 변환하려는 유사 배열 객체나 이터러블 객체. 이 매개변수는 필수
2. `mapFn` (선택사항): 요소를 변환할 때 사용할 매핑 함수. 이 함수는 각 요소에 대해 호출되며, 변환된 값을 반환. 이 매개변수를 지정하지 않으면 배열은 변환되지 않은 상태로 생성.
3. `thisArg` (선택사항): `mapFn`에서 사용할 `this` 값을 지정. 이 매개변수를 사용하면 `mapFn` 내에서 `this`를 설정할 수 있음.

예제코드

```jsx
// 문자열을 배열로 변환
const str = "hello";
const strArray = Array.from(str);
console.log(strArray); // ['h', 'e', 'l', 'l', 'o']

// Set 객체를 배열로 변환
const mySet = new Set([1, 2, 3, 4, 5]);
const setArray = Array.from(mySet);
console.log(setArray); // [1, 2, 3, 4, 5]
```

`Array.from()` 함수는 배열을 생성하거나 다른 객체를 배열로 변환하는데 유용한 메서드이며, 다양한 상황에서 활용할 수 있습니다.
