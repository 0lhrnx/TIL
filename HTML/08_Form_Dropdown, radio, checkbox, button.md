Form - Dropdown List
==
제한된 공간 안에서 여래개의 선택지를 선택할수 있도록 해주는 기능
## option 태그
+ 선택할수 있는 것들 즉, 각각의 것들을 선택지로 정의한 것
    + option은 select태그와 함께 사용한다


## option value

```
<option value="black">검정</option>
검정 이 아닌 black을 전송을 하고 싶을때 쓰는 속성 
```

## multiple 속성 
+ 사용자가 여러개의 항목을 선택하고 싶을 때 사용

<br>

Form - radio
==
## radio 버튼
+ 두개 동시에 누를수 있음

+ 네임값이 같은 것들끼리 groupng이 되는 것이고 같은 그룹에 속하는 것 중에 하나가 선택되면 나머지의 선택이 해제되는 형태

### value
+ 어떤 값이 돼야 되는지는 value로 적어줘야 함

<br>

Form - checkbox
## checkbox
+ 같은 네임을 가지고 있는 여래 개의 컨트롤을 다중으로 선택할 수 있다

### checked 
+ 기본적으로 어떠한 항목이 선택되고 싶다

<br>

Form - button
==
## Form Button
+ button은 html에서 순수하게 쓸 수 없다
    + 기본적으로 이름이 없기 때문에 직접 value를 써서 이름을 지정해줘야 한다.

## reset
+ ``<input type="reset">`` 

+ 사용자가 입력했던 모든 정보가 reset(재설정)된다