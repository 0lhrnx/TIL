# useNavigate

페이지를 이동할 때 사용된다.

## `<Link> </Link>` 와 useNavigate의 차이

- 단순하게 이동만 시켜야 하는 경우 Link를 사용한다.

- 특정 이벤트가 동작하도록 하거나 추가적인 로직이 필요한 경우 useNavigate를 사용한다.

## 사용방법

1. react-router-dom으로부터 useNavigate를 import 해온다.

```js
import { useNavigate } from "react-router-dom";
```

<br>

2. useNavigate를 호출해온다.

```js
const navigate = useNavigate();
```

<br>

3. 클릭 이벤트와 함께 사용한 예시이다.<br>
   버튼을 클릭했을 때 `/abuot`페이지로 이동 시킬 수 있다.

```js
<button
  onClick={() => {
    navigate("/about");
  }}
>
  어바웃 페이지로 이동하기
</button>
```

<br>

navigate 함수의 인자로 -1과 같은 숫자를 넣어서 이전 페이지로 이동시킬 수도 있다.

```js
<button
  onClick={() => {
    navigate(-1);
  }}
>
  이전 페이지로 이동하기
</button>
```
