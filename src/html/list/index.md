---
layout: home
title: "html5"
keyword: "html5"
description: "html을 학습합니다."
---

# 목록 및 표출력
메뉴 및 데이터등 다수의 데이터를 출력할 수 있는 테그들을 학습합니다.

## [목록](list)
목록은 동일한 유형의 데이터를 순차적으로 화면에 표시를 할 수 있는 방법입니다.
목록은 크게 2가지로 나누어 집니다.

* 순서가 있는 목록
* 순서가 없는 목록

## [테이블](table)
테이블은 다수의 데이터를 출력합니다.

* 테이블 구성
* 테이블 합치기



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
