# Generic

함수 또는 클래스를 정의할 때 타입을 명시하여 하나의 타입만이 아닌 다양한 타입을 사용할 수 있도록 하는 기법

```ts
function helloGeneric<T>(message: T): T {
  return message;
}

helloGeneric<string>("mark");

helloGeneric<number>(18);

helloGeneric<boolean>(true);
```
