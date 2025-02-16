# useMemo

컴포넌트의 성능을 최적화 하는데 사용되는 훅이다.

- useMemo에서 memo는 memoization으로 동일한 계산의 반복 수행을 제거하여 프로그램 실행 속도를 빠르게 하는 기술이다.

```js
const value = useMemo(() => {
  return calculate();
}, [item]);
```

- 첫 번째 인자: 콜백 함수
- 두 번째 인자: 의존성 배열

> 의존성 배열에 빈 배열을 넣는다면 useEffect처럼 마운트 될 때만 값을 계산하고 그 이후론 계속 memoization값을 꺼내와 사용한다.
