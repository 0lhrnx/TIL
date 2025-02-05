# Axios란?

브라우저, Node.js를 위한 Promise API를 활용하는 HTTP 비동기 통신 라이브러리이다.

## Axios VS Fetch API

```js
//fetch
const url ='http://localhost3000/test`
const option ={
   method:'POST',
   header:{
     'Accept':'application/json',
     'Content-Type':'application/json';charset=UTP-8'
  },
  body:JSON.stringify({
  	name:'sewon',
    	age:20
  })

  fetch(url,options)
  	.then(response => console.log(response))
```

```js
//axios
const option ={
  url ='http://localhost3000/test`
   method:'POST',
   header:{
     'Accept':'application/json',
     'Content-Type':'application/json';charset=UTP-8'
  },
  data:{
  	name:'sewon',
    	age:20
  }

  axios(options)
  	.then(response => console.log(response))
```

동일한 기능을 수행하는 코드이다.

두 코드의 차이점은

- Fetch() 는 body 프로퍼티를 사용하고, axios는 data 프로퍼티를 사용한다.

- Fetch의 url이 Fetch()함수의 인자로 들어가고, axios에서는 url이 option 객체로 들어간다.

- Fetch에서 body부분은 stringify()로 되어진다.

`이처럼 axios는 HTTP 통신의 요구사항을 컴팩트한 패키지로써 사용하기 쉽게 설계 되었다.`
