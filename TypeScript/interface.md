# interface

상호 간에 정의한 약속 혹은 규칙

```ts
interface User {
  age: number;
  name: string;
  gender?: "F" | "M"; // ?를 붙이면 써도 되고 안써도 된다.
  readonly birthYear: number; // readonly는 읽기 전용으로 값을 바꿀 수 없다.
}

let user: User = {
  age: 18,
  name: "leesan",
  gender: "M",
  birthYear: 2008,
};

user.gender = "F";
user.birthYear = 2007; // error
```
