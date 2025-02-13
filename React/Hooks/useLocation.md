# useLocation란?

현재 페이지의 정보를 가져오는데 사용한다.

## 5개의 키값을 가지고 있다.

`https://example.com/products?category=electronics#top%EB%9D%BC%EB%A9%B4`

- pathname : 현재 URL의 경로 부분을 나타낸다.

  - 위 URL에서 pathname은 /products이다.

- search : 현재 URL의 쿼리 파라미터를 나타낸다.

  - 위 URL에서 search는 ?category=electronics이다

- hash : 헌재 URL의 해시 부분을 나타낸다.

  - 위 URL에서 hash는 #top이다

- state : 이 프로퍼티는 라우팅된 컴포넌트로 전달되는 상태 객체를 나타냅니다.

  - 이전 경로에서 새로운 경로로 이동할 때 상태를 함께 전달하고 싶을 때 사용될 수 있습니다.

- key : 이 프로퍼티는 라우팅된 위치의 고유한 식별자를 나타냅니다.
  - React Router는 각각의 라우트 변경에 대해 고유한 키를 생성하여 라우팅된 컴포넌트의 인스턴스를 추적합니다.
