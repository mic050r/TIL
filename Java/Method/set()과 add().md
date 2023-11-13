# `ArrayList`에서 `set()` 메서드와 `add()` 메서드 사용법

## 1. `set(int index, E element)`

`set()` 메서드는 `ArrayList`에서 지정된 인덱스에 해당하는 요소를 주어진 요소(`element`)로 교체하는 역할을 합니다. 즉, 해당 인덱스에 저장된 요소를 변경하는 메서드입니다.

```java
ArrayList<String> list = new ArrayList<>();
list.add("A");
list.add("B");
list.add("C");

// 인덱스 1에 해당하는 요소를 "D"로 변경
list.set(1, "D");

// 변경 후 리스트: ["A", "D", "C"]

```

## 2. `add(E element)`

`add()` 메서드는 `ArrayList`에 주어진 요소(`element`)를 맨 뒤에 추가하는 역할을 합니다. 즉, 리스트의 가장 마지막에 요소를 추가하는 메서드입니다.

```java
ArrayList<Integer> numbers = new ArrayList<>();
numbers.add(1);
numbers.add(2);
numbers.add(3);

// 리스트의 끝에 4를 추가
numbers.add(4);

// 추가 후 리스트: [1, 2, 3, 4]

```

`add(E element)` 메서드는 리스트의 크기를 동적으로 늘려서 요소를 추가하므로, 요소를 삽입하려는 위치에 제한이 없습니다. 그리고 이 메서드는 리스트에 요소를 추가할 때마다 리스트의 크기가 증가하게 됩니다.

따라서, `set()` 메서드는 지정된 인덱스에 해당하는 요소를 변경하고, `add()` 메서드는 리스트의 끝에 새로운 요소를 추가합니다. 두 메서드는 서로 다른 역할을 수행하므로, 사용 목적에 따라 적절하게 선택하여 사용해야 합니다.
