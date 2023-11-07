# toPrecision()과 toFixed() 차이점

`toPrecision()`과 `toFixed()`는 모두 숫자를 문자열로 변환하는 메서드입니다. <br>
그러나 두 메서드는 사용하는 방식과 결과물에 차이가 있습니다.

## toPrecision() 함수

**toPrecision():** `toPrecision()` 메서드는 숫자를 지정한 유효 자릿수로 변환하여 문자열로 반환합니다. <br>
유효 자릿수는 정수부와 소수부의 자릿수를 모두 포함한 전체 자릿수입니다.<br>
이 메서드는 숫자를 반올림하거나 반내림하여 지정한 유효 자릿수로 표현합니다.<br>
필요에 따라 지수 표기법이 사용될 수 있습니다.<br>

```
const num = 3.14159;
console.log(num.toPrecision(4)); // "3.142"
console.log(num.toPrecision(2)); // "3.1"
```

## toFixed() 함수

**toFixed()**: toFixed() 메서드는 숫자를 지정한 소수점 자릿수로 변환하여 문자열로 반환합니다. <br>
이 메서드는 숫자를 반올림하여 지정한 소수 점 자릿수까지 표현합니다. <br>
반환된 문자열은 지정한 소수점 자릿수만큼의 길이를 가지게 됩니다. 필요에 따라 0이 추가됩니다.<br>

```
const num = 3.14159;
console.log(num.toFixed(2)); // "3.14"
console.log(num.toFixed(0)); // "3"
```

## 요약

**요약하면, toPrecision()은 유효 자릿수를 기준으로 숫자를 표현하는 반면, toFixed()는 소수점 자릿수를 기준으로 숫자를 표현합니다.**
<br>
toPrecision()은 정수부와 소수부의 자릿수를 모두 고려하여 반올림하고, toFixed()은 소수점 자릿수까지만 반올림하여 표현합니다. <br>
따라서 사용 목적에 맞게 유효 자릿수 또는 소수점 자릿수를 선택하여 적절한 메서드를 사용할 수 있습니다.
