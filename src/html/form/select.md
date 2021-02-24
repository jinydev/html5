---
layout: home
title: "html5"
keyword: "html5"
description: "html을 학습합니다."
---

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



##### select
여록 목록중 하나를 선택합니다.

```html
<select>
    <option></option>
    <option></option>
    <option></option>
</select>
```

* 속성
기본값은 1개만 선택됩니다. 
여러개의 선택을 할 경우에는 multiple 속성을 같이 지정을 합니다.
여러개의 값을 선택할 수 있습니다.

* 옵션

값을 


* optgroup
여러개의 항목이 많을때, 그룹을 지정할 수 있습니다.
그룹명을 출력할때는 `label` 속성을 지정합니다.
```html
<select>
    <optgroup label="서울">
        <option></option>
        <option></option>
        <option></option>
    </optgroup>
    <optgroup label="경기">
        <option></option>
        <option></option>
        <option></option>
    </optgroup>
</select>
```

라벨로 표시되는 텍스트는 선택할 수 없습니다.

그룹으로 묽인 옵션은 `들여쓰기` 형태로 표현됩니다.


