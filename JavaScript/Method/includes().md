# includes() 함수의 사용법

JavaScript의 **`includes()`** 함수는 배열이나 문자열에 특정 요소나 문자열이 포함되어 있는지를 확인하는 데 사용됩니다. 이 함수는 불리언 값을 반환합니다 (true 또는 false).

**배열에서의 `includes()` 사용**

```jsx
const array = [1, 2, 3, 4, 5];

console.log(array.includes(3)); // true
console.log(array.includes(6)); // false
```

위의 예제에서 `includes(3)`은 배열 `array`에 3이 포함되어 있는지를 확인합니다. `includes(6)`은 6이 배열에 포함되어 있는지를 확인하며, 위의 배열에는 6이 없으므로 `false`를 반환합니다.

**문자열에서의 `includes()` 사용**

```jsx
const string = "Hello, World!";

console.log(string.includes("Hello")); // true
console.log(string.includes("foo")); // false

```

위의 예제에서 `includes("Hello")`는 문자열 `string`에 "Hello"가 포함되어 있는지를 확인합니다. `includes("foo")`는 문자열에 "foo"가 포함되어 있는지를 확인하며, 위의 문자열에는 "foo"가 없으므로 `false`를 반환합니다.

**`includes()`** 함수는 대/소문자를 구분합니다. 따라서 대소문자를 구분하지 않고 포함 여부를 확인하려면 문자열을 모두 소문자나 대문자로 변환한 후에 **`includes()`** 함수를 사용해야 합니다.

```jsx
const string = "Hello, World!";

console.log(string.toLowerCase().includes("hello")); // true
```

위의 예제에서 **`toLowerCase()`** 메서드를 사용하여 문자열을 소문자로 변환한 후에 **`includes("hello")`**를 호출하면 대소문자를 구분하지 않고 "hello"가 포함되어 있는지를 확인할 수 있습니다.
