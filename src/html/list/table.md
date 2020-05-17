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





## 테이블
---
테이블은 `<table>` 요소로 지정을 합니다.

### 테이블 속성

```html
<table width="100%" boarder=1 summary="요약내용">
</table>
```

* width : 가로폭
width의 값은 고정된 px와 %를 모두 사용이 가능합니다. 하지만, %로 사용을 하는 것을 추천합니다. 페이지의 전체사이즈가 변경이 될때, 고정 px값은 문제가 발생할 수 있습니다.

* border : 선의 굵기

* summary : 표의 요약을 말합니다. 브라우저에 표시를 하지 않고, 시각장애인에게 읽혀지는 내용을 말합니다. 즐거리와 같습니다.


> 실제적인 디자인은 속성을 사용하는 것보다 CSS를 통하여 꾸미게 됩니다.


### caption 테그
caption은 표의 제목에 해당하며, table 테그 다음에 위치를 합니다.

켑션의 특징은 `가운데 정렬`로 표시 됩니다.




### 열(cols)
위에서 아래로 

* colgroup :
* col :

```html
<table>
    <colgroup>
        <col width="25%">
        <col width="25%">
        <col width="25%">
        <col width="25%">
    </colgroup>
</table>
```

테이블 한줄에 들어가는 열의 갯수만큼 col을 지정합니다.


### 행(rows)
가로줄을 말합니다.


### 머리말
thead

특징 : 가운데 정렬, 굵은 글씨로 표시됩니다.

제목셀인 `th`로 사용을 합니다. th는 tbody, tfoot에서도 사용이 가능합니다.

```html
<thead>
    <tr>
        <th>제목1</th>
        <th>제목2</th>
        <th>제목3</th>
        <th>제목4</th>
    </tr>
</thead>
```

### 본문
tbody


```html
<tbody>
    <tr>
        <td>내용1</td>
        <td>내용2</td>
        <td>내용3</td>
        <td>내용4</td>
    </tr>
</tbody>
```


### 하단
tfoot


```html
<tfoot>
    <tr>
        <td>내용1</td>
        <td>내용2</td>
        <td>내용3</td>
        <td>내용4</td>
    </tr>
</tfoot>
```

굵은 글자로 표시하고자 할때에는 td 대신에 th로도 사용할 수도 있습니다.

```html
<tfoot>
    <tr>
        <th>합계</th>
        <td>-</td>
        <td>-</td>
        <td>5050</td>
    </tr>
</tfoot>
```

### 셀 합치기

```html
<table>
    <tr>
        <tr>셀1</td>
        <tr>셀2</td>
        <tr>셀3</td>
        <tr>셀4</td>
    <tr>
    <tr>
        <tr>셀5</td>
        <tr>셀6</td>
        <tr>셀7</td>
        <tr>셀8</td>
    <tr>
    <tr>
        <tr>셀9</td>
        <tr>셀10</td>
        <tr>셀11</td>
        <tr>셀12</td>
    <tr>
</table>
```

#### 열 합치기 (colspan)
열이 합쳐 질때는 `오른쪽`에서 `왼쪽`으로 합쳐지게 됩니다.
합쳐지는 열은 테이블 셀에서 제거를 하과, 합치고자 하는 셀에 colspan 값을 지정합니다.



#### 행 합치기 (rowspan)
행은 `위`에서 `아래`로 합치게 됩니다.


```html
<table>
    <tr>
        <tr rowspan=2>셀1</td>
        <tr>셀2</td>
        <tr>셀3</td>
        <tr>셀4</td>
    <tr>
    <tr>
        <!-- <tr>셀5</td> -->
        <tr>셀6</td>
        <tr>셀7</td>
        <tr>셀8</td>
    <tr>
    <tr>
        <tr>셀9</td>
        <tr>셀10</td>
        <tr>셀11</td>
        <tr>셀12</td>
    <tr>
</table>
```

셀5번을 삭제하고 셀1에 rowspan값을 지정합니다.





