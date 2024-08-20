Form - 기본
==
+ 사용자가 입력한 정보를 서버로 전송할 때 사용하는 것들

## ``input 태그``
+ 사용자로부터 정보를 입력받을 수 있는 태그

+ type라는 속성으로 "text"를 하면 사용자로부터 문자 정보를 받을 수 있는 박스가 생김
    + input type="text"
+ type라는 속성에 "password"를 사용하면 글씨가 가려짐
    + input type="password"

+ type라는 속성에 "submit"을 사용하면 제출 버튼이 생김
    + input type="submit"

## ``submit 버튼 ``
 + 비밀번호, 아이디 입력 후 어떤 버튼 누르면 우리가 입력한 정보가 서비스로 넘어감 

## ``Form 태그``

 ### **action 속성**
+ 사용자가 입력한 정보들이 submit버튼을 눌렀을 때 어디로 보낼 것인가

<br>

각각의 control에 이름 정해주기
==
```
<p>아이디: <input type="text" name ="id"></p>
<p>비밀번호: <input type="password" name ="pwd"></p>
<p>주소: <input type="text" name ="address"></p>
```

 + 각각의 control에 아이디는 id, 비밀번호 pwd 주소는 address 이런식으로 이름을 줬기 때문에 서버쪽으로 전송할 때 바로 이 각각의 이름의 값으로 데이터가 전송되

