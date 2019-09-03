# Select
여러개의 값을 선택할 수 있습니다.

```html
<select name="" id="">
    </select>
```

## 선택

```html
<select name="" id="">
    <option value="korean">한국어</option>
</select>
```

## 기본값

```html
<select name="" id="">
    <option value="korean">한국어</option>
    <option value="english">영어</option>
</select>
```

## 다중선택
multiple 속성을 넣어 다중 선택이 가능하도록 할 수 있습니다.


## 그룹지정
optgroup 을 이용하여 선택되는 항목을 그룹을 정할 수 있습니다.

label값을 추가 할 수 있습니다.

```html
<select name="" id="">
    <optgroup label="아시아">
        <option value="korean">한국어</option>
    </optgroup>
    <optgroup label="북미">    
        <option value="english">영어</option>
    </optgroup>
    
</select>
```


