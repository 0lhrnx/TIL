# useCallback이란?

컴포넌트 성능을 최적화 시켜주는 도구이다.

## useMemo와 차이점

- useMemo는 값을 Memoization한다.

- useCallback은 함수를 Memoization한다.

---

```js
const memoizedCallback = useCallback(() => {
  doSomething(a, b);
}, [a, b]);
```

useCallback은 두 개의 인자를 받는다

- 첫 번째 인자로는 Memoization 해 줄 콜백함수를 받는다.

- 두 번째 인자로는 의존성 배열을 받는다.
