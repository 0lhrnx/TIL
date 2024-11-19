# State란?

컴포넌트의 상태를 말한다.

# useState란?

컴포넌트의 상태를 간편하게 생성하고 업데이트 해주는 도구를 제공한다.

```js
const [state, setState] = useState(0); // 초기값을 0으로 초기화
```

컴포넌트의 현재 상태 값은 state 라는 변수에 들어있고 state를 변경하고 싶으면 setState 함수를 이용해서 변경할 수 있다. 여기서 state랑 useState이름은 아무거나 해도 상관 없다.

setState를 이용해서 state를 변경하면 해당 컴포넌트는 화면에 다시 렌더링 된다.
