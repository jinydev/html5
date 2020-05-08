---
layout: home
title: "html5"
keyword: "html5"
description: "html을 학습합니다."
---

# 이름 붙이기
여러개의 입력을 받은 폼을 작성할 경우, 입력 내용을 구분하기 어렵습니다.

## 이름

```html
이름:
<input type="text">
```

## 라벨명

```html
<label for="">이름:</label>
<input type="text">
```
### for 속성
라벨과 입력폼의 focus를 일치를 합니다.

```html
<label for="firstname">이름:</label>
<input type="text" id="firstname">
```

for의 속성값과 동일한 이름으로 input 테그에 아이디를 설정합니다.

라벨을 클릭하면 자동으로 input 폼으로 초점이 이동하는 것을 확인 할 수 있습니다.


