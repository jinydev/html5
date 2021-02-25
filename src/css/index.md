---
layout: css
title: "CSS - 웹사이트 디자인하기"
keyword: "html5"
description: "html을 학습합니다."
---

# CSS
---
CSS는 `cascading style sheets` 의 약자 입니다. html을 꾸미기 위한 `선언적` 언어라고 할 수 있습니다.

<br>



## 공간영역

html 문서를 꾸미기 위한 공간 영역에 대해서 알아 봅니다.

* [block 영역](./tag/div)
* [inline 영역](./tag/span)

* 



## 버전
---
CSS는 1->2->3버전 까지 존재합니다.

### CSS 모듈


### 브라우저 접두사
브라우저별 css를 적용하는 접두사(prefix) 입니다.

* -webkit-
* -moz-
* -o-
* -ms-

브라우저를 자동으로 붙여주는 `prefix-free.js` 가 있습니다.



## 적용방법
css를 html 문서에 적용하는 방법은 3가지입니다.

테그에 직접 style 속성을 이용하여 적용하는 방법 입니다.

html 문서 내부에 style 테그를 이용하여 적용을 하는 방법입니다.

## 외부파일
`link` 테그를 이용하여 외부의 별도 파일을 읽어서 처리를 하는 방법입니다.

별도록 작성된 파일을 구성합니다.

### 확장자
---
별도로 작성된 스타일시트 파일은 `.css`확장자를 가지고 있습니다.

style.css 파일을 생성합니다.
```css
h1 {
    color:red;
}
```

### 파일연결
작성한 style.css 파일을 연결합니다.

```html
<link rel="stylesheet" href="style.css">
```

외부에 작성한 style.css 파일을 html 문서에 삽입을 합니다.
html의 head 영역에 작성을 합니다.

## 직접작성
html 문서에 직접 스타일 시트를 적용합니다. 문서에 직접 스타일 시트를 적용하기 위해서는 `style` 테그를 사용하여야 합니다.

```html
<style>
    h1 {
        color:red;
    }
</style>
```

기본적으로 head영역에 작성을 합니다. 하지만, 그외 지역에 설정을 하여도 스타일 시트가 적용이 됩니다.

head 이외의 영역에서 적용을 할 때에는 선언 위치가 중요합니다. html을 순차적으로 읽어 드리면서 적용이 됩니다.


## [인라인](inline)




## 참고

w3schools.com


