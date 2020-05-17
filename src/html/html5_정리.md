---
layout: home
title: "html5"
keyword: "html5"
description: "html을 학습합니다."
---

# html5
기존 html4보다 html5는 좀더 다양한 테그들이 추가 되어 있습니다.


## 레이아웃 요소들

### header 요소
문서의 제일 상단 부분을 의미 합니다.

기존 html4 에서는 

```html
<div id="header">
    상단영역...
</div>
```

html5 에서는 header 테그를 사용합니다.

```html
<header>
    상단영역...
</header>
```

해더 영역에는 서브메뉴들을 위한 nav 테그를 삽입하여 사용할 수 있습니다.

* lnb : local navigation bar
* gnb : global navigation bar


### nav 요소
네비게이션 내용등을 표현합니다.


```html
<div id="snb">
</div>
```

html5 에서는 nav 테그를 사용합니다.

```html
<nav>
    메뉴내용
</nav>
```

### main 요소
본문에 해당되는 내용입니다.
main은 페이지당 하나만 존재합니다. 또한 다른 header나 footer 안에 들어가지 않습니다.

html4 에서 자주 사용하던

```
<div id="content">
</div>
```

와 같이 처리하던 것을 main 테그로 처리합니다.

```html
<main>

</main>
```

### section
---
같은 성격의 내용들을 묽어서 표현할때 처리 합니다.

<br>

### article
---
독립적인 내용의 영역을 구현할때 사용을 합니다.

<br>

### footer
---
문서의 하단을 표현 합니다.


<br>

## 테이블5

테이블의 width 속성이 제외 되었습니다. 스타일로 대체를 하여 처리를 합니다.




### summary
html5에서 summary 속성 제외됨
대신 caption 테그 안에 삽입을 하여 사용하는 것은 가능합니다.

```html
<table>
    <caption>
        테이블 제목
        <summary> 요약글 </summary>
    </caption>
</table>
```

details 테그를 이용하여 summary를 같이 묶어서 처리를 할 수 있습니다.
화살표 형태로 표시되고, 클릭시 펼쳐지게 됩니다.
```html
<table>
    <caption>
        <details>
            테이블 제목
            <summary> 요약글 </summary>
        </details>
    </caption>
</table>
```

### col
html5 에서는 col의 속성인 width가 제외 되었습니다. 대신 스타일로 사이즈를 지정할 수 있습니다.



## figure / figcaption
html5에서 새롭게 등장한 요소입니다.

멀티미디어 요소의 설명을 넣을때 사용합니다.

```html
<figure>
    <img src="이미지.png" alt="">
    <figcaption>
        설명내용 구성
    </figcaption>
</figure>
```

alt 대체택스트를 figcaption 영역의 내용으로 대체.





## video, audio
html5 요소

영상과 음향을 제어합니다.

### video

```html
<video>
    <source src="sample.mp4">
</video>
```

#### controls
제어도구가 같이 표시 됩니다.

```html
<video controls>
    <source src="sample.mp4">
</video>
```

#### autoplay

```html
<video controls autoplay>
    <source src="sample.mp4">
</video>
```

#### loop


```html
<video controls autoplay loop>
    <source src="sample.mp4">
</video>
```


#### preload
데이터릴 미리 사전에 다운로드 받습니다.
* auto
* metadata
* none

```html
<video controls autoplay loop preload="auto">
    <source src="sample.mp4">
</video>
```

#### width
비디오의 사이즈를 지정합니다.

```html
<video controls autoplay loop preload="auto" width="500px">
    <source src="sample.mp4">
</video>
```


### 소리





