---
layout: home
title: "html5"
keyword: "html5"
description: "html을 학습합니다."
---

# 테이블
테이블 테그를 이용하여 그리드 데이터를 표현할 수 있습니다.

## table 테그
html에서 표를 생성하는 테그 입니다.  
테이블은 외각은 `table`테그를 사용합니다.

```html
<table>
</table>
```
위의 예제는 비어있는 테이블 입니다.  

`table` 테그는 기본적으로 2개의 테그를 포함합니다. `tr`테그는 가로줄을 의미하며
`td`테그는 셀을 의미합니다.

### tr
`tr`테그는 테이블에서 한줄을 의미 합니다.  

```html
<table>
    <tr></tr>
    <tr></tr>
</table>
```

위의 예제는 테이블은 2개의 줄을 포함합니다.  

### td
`td`테그는 테이블 한줄에 있는 셀 데이터를 의미합니다.

```html
<table>
    <tr>
        <td>내용1</td>
        <td>내용2</td>
        <td>내용3</td>
    </tr>
    <tr>
        <td>내용4</td>
        <td>내용5</td>
        <td>내용6</td>
    </tr>
</table>
```

`열` 과 `행`을 포함하는 데이터 테이블이 생성이 되었습니다.

## 데이터 영역
html5는 테이블 영역을 꾸밀수 있는 몇개의 테그들이 추가 되었습니다. 
실제 적인 데이터의 본체를 구별하기 위해서 `tbody` 테그를 추가합니다.

```html
<table>
    <tbody>
    <tr>
        <td>내용1</td>
        <td>내용2</td>
        <td>내용3</td>
    </tr>
    <tr>
        <td>내용4</td>
        <td>내용5</td>
        <td>내용6</td>
    </tr>
    </tbody>
</table>
```

## 상단영역
보통 테이블의 첫번째 줄은 각 셀의 의미를 담고 있는 제목으로 사용 되는 경우가 많습니다.
html5에서는 테이블 내부의 영역을 구분하여 제목행을 구별할 수 있는 `thead`테그를 지원합니다.

```html
<table>
    <thead>
    <tr>
        <td>제목1</td>
        <td>제목2</td>
        <td>제목3</td>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>내용1</td>
        <td>내용2</td>
        <td>내용3</td>
    </tr>
    <tr>
        <td>내용4</td>
        <td>내용5</td>
        <td>내용6</td>
    </tr>
    </tbody>
</table>
```

## 하단설정
html5는 테이블의 하단 영역을 추가할 수 있습니다. 
`tfoot`테그를 사용합니다.

```html
<table>
    <thead>
    <tr>
        <td>제목1</td>
        <td>제목2</td>
        <td>제목3</td>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>내용1</td>
        <td>내용2</td>
        <td>내용3</td>
    </tr>
    <tr>
        <td>내용4</td>
        <td>내용5</td>
        <td>내용6</td>
    </tr>
    </tbody>
    <tfoot>
    <tr>
        <td>하단1</td>
        <td>하단2</td>
        <td>하단3</td>
    </tr>
    </tfoot>
</table>
```

## 제목
html5의 테이블은 제목을 별도의 테그로 설정을 할 수 있습니다.
`caption`테그를 삽입합니다.

```html
<table>
    <caption>제목입니다.</caption>
    
    <thead>
    중간생략...
    </thead>
    <tbody>
    중간생략...
    </tbody>
    <tfoot>
    중간생략...
    </tfoot>
</table>
```

`caption`테그는 테이블 테그안에, 상단에 작성을 합니다.

## colgroup
컬럼열의 그룹을 설정할 수 있습니다.


## 테이블 속성
테이블 테그에 속성을 이용하여 표를 꾸밀 수 있습니다.

### 테두리
`border` 속성은 테이블의 테두리를 설정합니다.

```html
<table border="1">
    중간생략
</table>
```

## 합치기
작성된 표의 일부분을 합치는 기능을 제공합니다.

### colspan
가로로 걸치는 셀의 갯수
`colspan` 셀의 너비를 지정합니다.

### rowspan
세로로 걸치는 셀의 갯수
`rowspan` 셀의 높이를 지정합니다.







