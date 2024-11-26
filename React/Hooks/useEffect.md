# useEffect란?

React component가 렌더링 될 때마다 특정 작업을 실행 할 수 있도록 하는 리액트 Hooks이다.

useEffect는 component가 mount 됐을 때, component가 unmount 됐을 때, component가 update 됐을 때 특정 작업을 처리 할 수 있다.

# 사용법

```js
useEffect { function, deps }
```

- function : 수행하고자 하는 작업

- deps : 배열 형태이며, 배열 안에는 검사하고 하는 특정 값 or 빈 배열

# useEffect 사용 방식

1.  Component가 mount 됐을 때 ( 처음 나타났을 때 실행 )

```js
useEffect(() => {
  console.log("마운트 될 때만 실행된다");
}, []);
```

컴포넌트가 화면에 가장 처음 렌더링 될 때 한 번만 실행하고 싶다면 deps 위치에 빈 배열을 넣어준다.

```js
useEffect(() => {
  console.log("렌더링 될 때 마다 실행된다");
});
```

만약 배열을 생략한다면 리렌더링 될 때마다 실행된다.

<br>

2. Component가 update 될 때 (특정 props, state가 바뀔 때)

```js
useEffect(() => {
  console.log(name);
  console.log("업데이트 될 때 실행된다");
}, [name]);
```

- 특정 값이 업데이트 될 때 실행하고 싶으 때는 deps위치에 배열 안에 검사하고 싶은 값을 넣어준다.

  3. Component가 unmount될 때(사라질 때)& update되기 직전에 실행

```js
useEffect(() => {
  console.log("effect");
  console.log(age);
  return () => {
    console.log("cleanUp");
    console.log(age);
  };
}, []);
```

`-` cleanUp 함수 반환(return 뒤에 나오는 함수이며 useEffect에 대한 뒤정리 함수라고 한다.)

`-` 언마운트 될 때만 cleanUp함수를 실행하고 싶으면 deps자리에 빈배열을 넣는다.

`-` 특정 값이 업데이트 되기 직전에 cleanUp함수를 실행하고 싶다면 deps에 검사하고 싶은 값을 넣어줍니다.
