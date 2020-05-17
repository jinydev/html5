


##### label
요소의 타이틀을 출력하고자 할때 사용합니다.

```html
<label>항목</label>
```

label을 폼 요소와 결합하여 사용시에는 선택 클릭의 영역이 넓혀 주게 됩니다.
요소와 결합을 할때는 for 속성을 사용합니다. for는 연결하는 폼요소의 id 값을 입력합니다.


```html
<label for="item">항목</label><input type="radio" id="item">
```


##### 레이블 표기법

* 명시적 레이블
id와 for를 이용하여 레이블을 연결합니다.
```html
<label for="item">항목</label><input type="radio" id="item">
```

* 암묵적 레이블
label 요소안에 input 테그만 넣는경우.
```html
<label><input type="checkbox"></label>
```
이 방법은 추천하지 않는 작성예 입니다. 

* 혼합형
id와 for가 1:1 로 연결이 되어 있습니다. 하지만, 입력 요소가 여러개인 경우 우선시 되는 입력요소만을 연결합니다.


```html
<label for="phone">연락처</label>
<select id="phone">
    <option>+82</option>
</select>

- <input type="text" title="번호자리1">
- <input type="text" title="번호자리2">
- <input type="text" title="번호자리3">
```

타이틀은 `툴팁`으로 나타나게 됩니다.

