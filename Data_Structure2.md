# Data Structure2

## dictionary

- .get(k) : 키 k에 연결된 값 반환

- .get(k, v) : 키 k에 연결된 값 반환, 키가 없으면 기본 값으로 v 반환

- .keys() : dictionary의 키를 모은 객체 반환

- .values() : dictionary의 값을 모은 객체 반환

- .items() : dictionary의 키/값 쌍을 모은 객체 반환

- .pop(k) : 키 k를 제거하고 연결된 값을 반환

- .pop(k, v) : 키 k를 제거하고 연결된 값을 반환, 키가 없으면 기본값으로 v 반환

- .clear() : dictionary 안의 모든 키, 값 제거


**from collection defaultdict (아주 유용)**

## set

- .add(x) : set에 x 항목 추가

- .clear() : set의 모든 항목 제거

- .remove(x) : set의 x 항목 제거

- .pop(x) : x 항목을 반환하고 해당 항목 제거

- .update(iterable) : iterable 안의 항목들 전부 