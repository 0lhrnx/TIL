# useParams란?

Parameter 값을 URL을 통해서 넘겨받은 페이지에서 사용할 수 있도록 해주는 것

```js
function App() {

  return (
  <div className="App">
      <Routes>
        <Route path="/detail/:id" element={<Detail />}/>
      </Routes>
  </div>
  );

function Product() {

  const productList =[
  {id : 0, name : Jorden1 Chicago, color: red},
  {id : 1, name : Jordan1 Oreo, color: black},
  {id : 2, name : Jorden1 Smokegrey, color: grey },
  ]

  const {id} = useParams();

  return (
  	<div className="product-list">
    	<h3> productList[id].name </h3>
      	<p> productList[id].color </p>
    </div>
  );
```

만약 URL이 /detail/0 이라면 Jorden1 Chicago하고 red인 것을 렌더링함.
