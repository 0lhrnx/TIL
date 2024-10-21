# 컴포넌트란?

- 재사용 가능한 UI 부품

- component라는 부품을 모아 하나의 화면을 만듦

  - 기존 html의 비효울적인 중복되는 코드 줄여줌!

- 쉽게 말하자면, HTML element들의 집합

## 장점

- 재사용성이 높다

- 유지보수성과 가독성이 높아진다

---

# components는 Javascript 함수다

- 어떤 경우에 우리는 함수를 만들까?

  - 특정 역할을 수행하게 하려고( features, pages )

  - 재사용 되는 로직을 모듈화해서 불필요한 반복 작업을 줄이려고( 좁은 범위의 components )

# 함수형 component와 클래스형 component

- 함수형 컴포넌트

  - state, lifeCycle 관련 기능 사용 불가능 (Hook을 통해 해결 가능)

  - 컴포넌트 선언이 편하다

  - input은 Props

  - output은 UI

- 클래스형 컴포넌트

  - class 키워드 필요

  - component로 상속을 받아햐 함

  - render() 메소드가 반드시 있어야 함

  - state, lifeCycle 관련 기능 사용 가능

## 주의

- 컴포넌트는 첫글자 무조건 대문자로 작성

![]()
