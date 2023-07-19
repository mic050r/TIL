# localStorage
JavaScript의 `localStorage`는 웹 브라우저에서 데이터를 클라이언트 측에 저장하기 위한 웹 스토리지 메커니즘입니다. 

**`localStorage`** 객체는 브라우저에 키-값 쌍으로 데이터를 영구적으로 저장할 수 있는 간단한 인터페이스를 제공합니다.

`localStorage`를 사용하면 사용자의 로컬 컴퓨터에 데이터를 저장하고, 브라우저 세션 또는 재시작 후에도 그 데이터를 유지할 수 있습니다. 이는 웹 애플리케이션에서 사용자의 환경 설정, 사용자 이름, 마지막 방문 시간 등을 저장하거나 다른 페이지 간에 데이터를 공유하는 데 유용합니다.

`localStorage`를 사용하기 위해 다음과 같은 메서드를 사용할 수 있습니다:

- **`localStorage.setItem(key, value)`**: 특정 키에 값을 저장합니다. 키와 값을 문자열로 지정해야 합니다.
- **`localStorage.getItem(key)`**: 특정 키에 저장된 값을 반환합니다.
- **`localStorage.removeItem(key)`**: 특정 키에 저장된 값을 제거합니다.
- **`localStorage.clear()`**: `localStorage`에 저장된 모든 값을 제거합니다.
- **`localStorage.length`**: `localStorage`에 저장된 키-값 쌍의 개수를 반환합니다.

**`localStorage`**를 사용하여 데이터를 저장하고 검색하는 예제에 대해 알아보겟습니다.

```jsx
// 데이터 저장
localStorage.setItem('username', 'John');
localStorage.setItem('email', 'john@example.com');

// 데이터 검색
const username = localStorage.getItem('username');
const email = localStorage.getItem('email');
console.log(username, email); // 출력: John, john@example.com

// 데이터 제거
localStorage.removeItem('email');

// 모든 데이터 제거
localStorage.clear();
```

`localStorage`는 문자열 형태로 데이터를 저장하기 때문에 객체나 배열과 같은 복잡한 데이터를 저장하려면 JSON.stringify()를 사용하여 문자열로 변환하고, 필요할 때 JSON.parse()를 사용하여 다시 객체로 변환해야 합니다.
