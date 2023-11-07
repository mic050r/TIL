# JSON 객체

**JSON (JavaScript Object Notation)** 은 데이터를 표현하기 위한 경량의 데이터 교환 형식입니다.
JSON은 텍스트 형식으로 구성되며, 사람과 기계 모두가 읽고 쓰기 쉬운 형태를 가지고 있습니다.
JSON은 JavaScript에서 사용되는 객체와 유사한 구조를 가지고 있으며, 다양한 프로그래밍 언어에서 지원되고 사용됩니다.

JSON 객체는 중괄호({})를 사용하여 정의되며, 키-값 쌍의 집합으로 구성됩니다.
각 키는 문자열로 작성되고, 키와 값은 콜론(:)으로 구분됩니다.
여러 개의 키-값 쌍은 쉼표(,)로 구분됩니다.
값은 다양한 데이터 유형을 가질 수 있으며, 객체, 배열, 문자열, 숫자, 불리언, null 등을 포함할 수 있습니다.

JSON 객체의 예시:

```
var person = {
  "name": "John",
  "age": 30,
  "city": "New York"
};
```

```
var car = {
  "make": "Toyota",
  "model": "Camry",
  "year": 2021,
  "isElectric": false,
  "features": ["GPS", "Bluetooth", "Backup Camera"]
};
```

위의 코드에서 person과 car는 JSON 객체입니다.
person 객체는 이름(name), 나이(age), 도시(city)와 같은 키-값 쌍으로 구성되어 있습니다.
car 객체는 자동차 제조사(make), 모델(model), 연도(year), 전기차 여부(isElectric), 특징(features)과 같은 키-값 쌍으로 구성되어 있습니다.
특히 features 키의 값은 배열로 구성되어 여러 개의 값을 가질 수 있습니다.

JSON 객체는 다양한 용도로 사용됩니다.
주로 서버와 클라이언트 간의 데이터 교환, 데이터 저장 및 전송 등에 활용됩니다.
JavaScript에서는 JSON.stringify() 메서드를 사용하여 JavaScript 객체를 JSON 문자열로 변환하고, JSON.parse() 메서드를 사용하여 JSON 문자열을 JavaScript 객체로 변환할 수 있습니다.
