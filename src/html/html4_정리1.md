---
layout: home
title: "html5"
keyword: "html5"
description: "html을 학습합니다."
---

## html 구조

### 시작요소
html 문서의 시작과 끝을 표시합니다.
```html
<html>
</html>
```

html 테그 안에는 2개의 영역이 존재 합니다.
`head` 영역과 `body` 영역입니다.

### head 영역
해드 영역은 head 테그를 사용합니다.

```html
<head>
</head>
```

헤드 요소에는 페이지를 꾸미기 위한 정보들을 삽입합니다.

대표적으로 css, js, meta, title 등이 있습니다.


### body 영역

바디 영역은 body 테그를 사용합니다.

```html
<body>
</body>
```

페이지가 그려지는 공간 입니다. 실제 브라우저로 보여지는 내용입니다.


### 완성된 구조
해드 영역과 바디 영역을 삽입하면 다음과 같은 구조가 됩니다.

```html
<html>
    <head> </head>
    <body> </body>
</html>
```

<br>

## 요소
---
테그를 통하여 요소를 정의 합니다.

테그는 `<`와 `>` 사이에 요소명을 지정합니다.

테그는 시작테그와 종료테그로 이루어 집니다.

종료 테그가 없는 요소들도 있습니다.


### 속성
요소는 테그명 이외에 속성값을 가질 수 있습니다.



## heading 요소
제목을 표현하는 요소를 말합니다.

글자의 크기에 따라서 6가지가 있습니다.

`H`요소는 블럭 속성을 가지고 있습니다.

h테그 안에는 `텍스트` 또는 `inline` 요소들만 포함할 수 있습니다.


계층적 표현
h는 계층적으로 표현하는 것이 바람직 합니다.

h1> h2> h3 > h4 > h5 > h6

H1 요소는 `한페이지`에 `한번만 사용`하는 것을 추천합니다.

굵은 글씨로 표현이 됩니다.

## 이미지 삽입하기
이미지를 삽입하기 위해서는 `<img>` 테그를 사용합니다.

### 이미지 위치
속성값으로 이미지의 위치를 지정해 주어야 합니다.

```html
<img src="logo.jpg">
```

이미지 파일명과 확장자를 같이 지정해 주어야 합니다.

#### 이미지의 종류
* jpg
* png
* gif

#### 이미지 경로위치
이미지를 지정할 때는 `경로`명도 정확히 지정을 해주어야 합니다.

* 현재위치
* 상대경로
* 절대경로

### 대체 텍스트
alt 속성을 부여하여 시각장애인이 인식할 수 있도록 대체 텍스트를 입력합니다.

만일 alt 값이 없어도 생략하지 말고 빈 내용으로도 넣어 주어야 합니다.

```html
<img src="logo.jpg" alt="">
```

대체 텍스트 설명 내용이 많을 경우 `longdesc` 속성을 이용합니다.

```html
<img src="logo.jpg" alt="간단한 설명" longdesc="descript.html">
```
> 파이어폭스, 마우스 오른쪽키 메뉴 -> 설명보기


```html
<img src="logo.jpg" alt="간단한 설명" >
<div style="position:absolute; left:-200%">
상세정보
</div>
```
하단에 대체 택스트 설명을 배치합니다. 일반인들은 보이지 않도록 position을 변경하여 안보이게 합니다. 하지만, 시각장애인들을 이를 읽을 수 있습니다.

> 주의 display:none 속성으로 하게 되면 인식이 되지 않아 
대체 택스트를 읽을 수 없습니다.



### 이미지의 사이즈 지정


<br>

## 앵커 연결
a 링크에 대해서 알아 봅니다.

### 링크 페이지
연결되는 링크는 href 속성을 부여하면 됩니다.

```html
<a href="사이트">이동합니다.</a>
```

* 외부 사이트 : http 또는 https 프로토콜을 포함한 전체 주소를 입력합니다.
* 절대 주소
* 상대주소

### 새창열기

```html
<a href="사이트" target="_blank">이동합니다.</a>
```

### 클릭확인
a 링크로 연결시
한번도 클릭한 적이 없는 경우에는 `파랑색`으로 표시됩니다.
한번 적속한 경우에는 `보라색`

### 밑줄
a 링크는 밑줄이 표시됩니다.

### 인라인
a 링크는 인라인 속성을 가지고 있습니다.
여러개의 링크를 작성시 한줄로 배치가 됩니다.

### 빈링크

```html
<a href=""> </a>
```
 - ie에서는 내컴퓨터가 선택됩니다.
 - 크롬에서는 반응을 하지 않습니다.


```html
<a href="#"> </a>
```
페이지 제일 상위로 스크롤이 이동하게 됩니다.



```html
<a href="#aaa"> </a>
```
id 값이 있는 컨덴츠가 있는 경우 스크롤을 이동하게 됩니다.


```html
<a href="#none"> </a>
```
지정한 id가 없는 경우, 반응을 하지 않고, 현재의 위치에 머무르게 됩니다.
목적지가 없기 때문에 반응을 하지 않습니다.

<br>

## Entity code
엔티티 코드는 `특수문자`를 `특별한 코드`로 표현을 하는 것입니다.
html 문법과 충돌하지 않고, 오류를 방지하기 위해서 사용을 합니다.

```html
&코드;
```

* ` ` - nbsp
* `<` - lt
* `>` - gt
* `` - middot
* `&` - amp
* `"` - quot

> 단일 따옴표는 entity code를 제공하지 않습니다.

<br>

## br
---
html에서는 엔터 다음줄을 브라우저에 직접 표현을 하지 않습니다.
엔터와 같은 다음줄을 출력하기 위해서는 `<br>`테그를 사용해야 합니다.

<br>

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



## 리스트
순서형, 비순서형, 

### 비순서형 목록 (Unordered List)
특징 li 마다 블릿이 제공됩니다.
연속적인 컨덴츠를 나열할때 용이합니다.

```html
<ul>
    <li>상위</li>
    <li>하위</li>
    <li>악세사리</li>
</ul>
```

> 주의:
ul 테그와 li 테그 사이에는 다른 요소의 테그를 삽입할 수 없습니다.
li와 li 사이에도 다른 요소의 테그를 삽입할 수 없습니다.

#### 중첩목록
li안에는 또다른 ul 목록을 넣을 수 있습니다.

목록이 중첩하게 되면 `들여쓰기` 형태로 표현이 됩니다.


### 순서형 목록 (Ordered List)
ol로 표시를 합니다.

```html
<ol>
    <li>1일차 코스</li>
    <li>2일차 코스</li>
    <li>3일차 코스</li>
</ol>
```

#### 중첩목록

```html
<ol>
    <li>1일차 코스
        <ol>
            <li>오전 일정</li>
            <li>오후 일정</li>
        </ol>
    </li>
    <li>2일차 코스</li>
    <li>3일차 코스</li>
</ol>
```


### 병합중첩
ul 목록 서브로 ol 목록을 삽입하거나, ol 목록에서 ul 목록을 서브로 삽입할 수도 있습니다.



### 정의형 목록
dl, dt, dd

사전적의미를 표현할때 자주 사용됩니다. 그외에는 잘 사용하지 않는 테그 입니다.


* dl : 정의형 목록 지정
defines a description list

* dt : 용어정의
defines terms 또는 name

* dd : 정의 설명
describes each term


```html
<dl>
    <dt>what is Web</dt>
    <dd>web is ....</dd>
    <dd>....</dd>
</dl>
```

dt /dd 는 순서대로 한개의 묽음으로 처리하여 작성을 해주어야 합니다.
dd는 한개 이상으로 반드시 같이 정의해 주어야 합니다.

```html
<dl>
    <dt>what is Web</dt>
    <dd>web is ....</dd>

    <dt>what is interner</dt>
    <dd>internet is ....</dd>
</dl>
```

dl은 여러개 쌍의 dt/dd를 포함할 수 있습니다.


<br>

## 폼(form)
폼은 온라인 서식을 구현할때 사용되는 요소들 입니다.

### form

```html
<form>
내용
</form>
```

폼 요소 자체가 브라우저에 표시를 하지 않습니다. 폼 요소안에 들어있는 내용만을 출력합니다.

#### 속성

* action : 폼이 전송하고자 하는 url

* method : 폼의 정보를 전달하는 방법
get/post로 선택합니다.



### fieldset
폼 요소의 그룹을 지정합니다. 필드셋을 지정하게 되면, 그룹화된 요소들 주위에 테두리가 표시됩니다.
필드셋과 같이 제목을 정의하기 위해서 legend 테그를 사용합니다.

```html
<form>
    <fieldset>
        <legend>필드셋 제목</legend>
        내용...
    </fieldset>
</form>
```


### 요소들
다양한 폼 요소가 존재합니다.

#### input

```html
<imput type="????">
```

타입에 종류별로 다르게 동작을 합니다.

##### text : 
글 입력상자, 한줄만 입력됩니다. 2줄이상의 글씨는 입력할 수 없습니다.

* readonly 속성을 부여하게 되면 편집이 불가능합니다.
* disabled : 비활성 상태로 표현합니다.
* maxlength : 글자의 입력을 제한합니다.

placeholder : html5에 추가된 기능입니다.


##### password : 
비밀번호 입력상자

입력하는 글자가 표시가 되지 않도록 점 또는 별 모양으로 암호화된 형태로 출력됩니다.
점 과 별은 브라우저 마다 틀리게 표현됩니다.


#### radio : 
단일 선택자
클릭하면 선택할 수 있도록 합니다. 복수의 여러개의 선택이 있을 경우 하나만 선택할 수 있습니다.

여러개를 선택할때는 name 속성을 통하여 그룹화 시켜야 합니다.

```
<input type="radio" name="sex" value="남자"> 남자
<input type="radio" name="sex" value="여자"> 여자
```

동일한 name 값을 지정하게 되면, 선택된 하나의 결과값을 서버로 전송할 수 있습니다.


##### checkbox : 
다중 선택자

하나만 선택할 수 있는 radio와 달리 여러개의 항목을 선택할 수 있습니다.


##### file : 
첨부파일
로컬 컴퓨터의 파일을 선택하여 서버로 전송을 합니다.

`파일선택` 버튼이 생성이 되는데, 버튼을 클릭하면 파일 선택창이 나타납니다.

`파일선택`의 타이블은 브라우저 또는 운영체제에 의해서 표시되는 텍스트 입니다. 임의적으로 변경을 하지 않습니다.

브라우저 마다 버튼의 디자인이 다르게 표시됩니다.

##### image : 
이미지 버튼

타입이 image로 선택할 경우에는 이미지 경로를 같이 지정해 주어야 합니다.

```html
<input type="image" src="이미지경로" alt="대체 텍스트">
```


##### submit
폼에 입력된 값을 서버로 전송을 합니다.

기본값은 `제출` 입니다. 텍스트를 변경하기 위해서는 value 값을 지정해야 합니다.

```
<imput type="submit" value="전송">
```

누르는 효과가 같이 에니메이션 동작이 표현됩니다.

##### reset
입력값이 전체 취소하여 초기화 하는 동작을 수행합니다.

```
<imput type="reset" value="취소">
```

##### button

범용적인 버튼을 구현합니다.

```html
<imput type="button" value="확인">
```

또는 button 테그를 통하여 표현을 할 수도 있습니다.

```html
<button>확인</button>
```

##### hidden
사용자에게 보이지 않는 입력폼을 말합니다.


##### textarea
여러줄의 글씨를 입력할 수 있는 요소 입니다.
다중 편집창

입력창의 크기를 지정할 때는 

* cols : 가로 텍스트 입력수, 가로폭

* rows : 세로 입력 수 , 높이
엔터의 갯수를 의미합니다.


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



## title
페이지의 제목을 표시하는 테그 입니다.head 안에 선언을 합니다.
브라우저 상단에 페이지 타이들 제목이 출력 됩니다.

```html
<title>페이지 제목입니다.</title>
```

낭독기에서도 제일 먼저 읽어 주는 것이 타이틀 입니다.

> 주의할점
타이틀에 특수문자는 삽입하지 않습니다.

```html
<title>현재위치 - 타이틀</title>
```

순서로 지정하는 것을 추천합니다.










