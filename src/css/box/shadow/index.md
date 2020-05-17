---
layout: home
title: "Box Shadow - Learn CSS"
keyword: "box-shadow, css, css3, html5"
description: "그림자 박스를 제작하기 위한 css에 대해서 학습합니다."
breadcrumb:
- css
- box
- shadow
---

> CSS3
## box-shadow

박스 영역에 그림자를 추가합니다.

```css
div {
    box-shadow: 3px 3px 3px #000;
}
```

> 예제코드 : ./dample/shadow10.html


첫번째 값
x축을 기반으로 그림자 위치

두번째값
y축 기반 그림자 위치

세번째값 
그림자 번지는 크기값

네번째값
그림자 색상
rgb 또는 rgba 모두 사용이 가능합니다.


## 안쪽 그림자
안쪽 부분에 그림자를 넣고자 할때에는 `inset` 값을 추가합니다.

```css
div {
    box-shadow: inset 3px 3px 3px #000;
}
```

## 그림자의 컨덴츠 영역
그림자는 다른 컨덴츠 요소에 영향을 미치지 않습니다.

그림자로 인하여 영역이 겹치는 문제가 있는 경우, 마진 또는 패딩값을 추가로 주어야 합니다.



