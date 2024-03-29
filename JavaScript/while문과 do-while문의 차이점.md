# while문과 do-while문의 차이점

**`while`** 문과 **`do-while`** 문은 둘 다 반복 작업을 수행하기 위한 제어문입니다. 그러나 두 문장 사이에는 동작 방식과 실행 순서에서 차이점이 있습니다.

## 1. **`while`** 문

- **`while`** 문은 반복되기 전에 조건식을 평가합니다. 조건식이 참(**`true`**)인 경우에만 반복 코드 블록이 실행됩니다.

### 1-1) 기본 구조

```jsx
while (조건식) {
  // 반복해서 실행할 코드
}
```

### 1-2) 예시코드

ex) 다음 JavaScript 코드는 변수 `i`가 1부터 100까지 증가하면서 숫자를 더하는 예시입니다.

```jsx
var i = 1;
var total = 0;
while (i <= 100) {
  total += i;
  i++;
}
console.log(total); // 5050
```

## 2. **`do-while`** 문

- **`do-while`** 문은 반복 코드 블록을 실행한 후에 조건식을 평가합니다. 조건식이 참인 경우 반복이 계속됩니다.
- 즉, **`do-while`** 문은 반복 코드 블록을 최소한 한 번은 실행하고, 그 후에 조건을 검사합니다.

### 2-1) 기본 구조

```jsx
do {
  // 반복해서 실행할 코드
} while (조건식);
```

### 2-2) 예시 코드

ex) 다음 JavaScript 코드는 변수 `i`가 1부터 100까지 증가하면서 숫자를 더하는 예시입니다.

```jsx
var i = 1;
var total = 0;
do {
  total += i;
  i++;
} while (i <= 100);
console.log(total); // 5050
```

## 주요 차이점

: 반복 조건을 검사하는 시점

- **`while`** 문은 조건을 먼저 평가하므로 조건이 거짓인 경우 아무 코드도 실행되지 않을 수 있습니다.
- **`do-while`** 문은 코드 블록을 최소한 한 번은 실행한 후에 조건을 검사하므로, 코드 블록은 반드시 한 번 이상 실행됩니다.

어떤 반복 작업을 수행해야 하는지와 조건을 언제 평가해야 하는지에 따라 **`while`**과 **`do-while`** 중 어떤 것을 선택할지 결정할 수 있습니다. 만약 코드 블록이 최소한 한 번은 실행되어야 하는 경우, **`do-while`**이 유용하며, 반면 조건에 따라 실행 여부가 결정되는 경우 **`while`**을 사용할 수 있습니다.
