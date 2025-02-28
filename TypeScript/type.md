# Type

Typescript에서는 Type을 지정할수 있다.

## Typescript 기본 타입들

```ts
// Number Type
const num: number = 1234;
```

```ts
// String Type
const str: string = "hi";
```

```ts
// Boolean Type
const b: boolean = false;
```

```ts
// Object Type
const obj: object = { name: "leesan", age: 18 };
```

```ts
// Array Type
const arr: number[] = [1, 2, 3];

const arr: Array<number> = [1, 2, 3];
```

```ts
// Tuple Type
const arr: [string, number] = ["hi", 123];
// 튜플은 배열의 길이가 고정되고 각 요소의 타입이 지정되어 있는 배열 형식
```

```ts
// Enum Type
enum color {
  red,
  blue,
  green,
}

const c: color = color.red;
// 특정 값들의 집합
```

```ts
// Any Type
let a: any = "hi";
a = 1234;
```

```ts
// Void Type
function sayHi(): void {
  console.log("hi");
}

const a: void = null;

const b: void = undefined;

// 변수에는 undefined와 null만 할당이 가능하고, 함수로 설정할 경우 리턴 값을 설정할 수 없다.
```

```ts
// Never Type
function invalid(message: string): never {
  throw new Error(message);
} // 항상 오류 발생

// never는 일반적으로 함수의 리턴 타입으로 사용되는데, 항상 오류를 출력하거나 리턴 값을 절대로 내보내지 않음을 의미
```

```ts
// Union Type
const u: string | number = "hi";

// 둘중의 아무거나 사용 가능
```
