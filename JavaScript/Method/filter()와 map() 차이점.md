#  filter()와 map() 차이점

**filter()** 와 **map()** 은 JavaScript 배열에서 각각 다른 용도로 사용되는 배열 메서드입니다. <br>
주요한 차이점은 다음과 같습니다:

## filter()
`filter()`: 이 메서드는 배열 요소를 필터링하여 새로운 배열을 반환합니다. <br>
주어진 함수의 조건을 만족하는 요소만 선택하여 반환합니다. <br>
즉, 원본 배열에서 조건에 맞는 요소만 남기고 나머지는 제외합니다.

```
const numbers = [1, 2, 3, 4, 5];

// 짝수만 필터링하여 새로운 배열 생성
const evenNumbers = numbers.filter(num => num % 2 === 0);
console.log(evenNumbers); // [2, 4]
```

## map()
`map()`: 이 메서드는 배열 요소를 변환하여 새로운 배열을 반환합니다. <br>
주어진 함수를 각 요소에 적용하여 변환된 값을 가진 새로운 배열을 생성합니다.<br>
원본 배열의 크기와 같은 크기의 새로운 배열을 생성하며, 각 요소에 대해 변환된 값을 가지게 됩니다.

```
const numbers = [1, 2, 3, 4, 5];

// 각 요소를 제곱하여 새로운 배열 생성
const squaredNumbers = numbers.map(num => num ** 2);
console.log(squaredNumbers); // [1, 4, 9, 16, 25]
```

## 요약

요약하자면, `filter()`는 조건에 맞는 요소를 선택하여 배열을 필터링하고, `map()`은 각 요소를 변환하여 새로운 배열을 생성.<br>
`filter()`는 조건에 따라 요소를 선택하는 데 사용되고, `map()`은 각 요소를 변환하는 데 사용.
