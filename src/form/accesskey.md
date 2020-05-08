---
layout: home
title: "html5"
keyword: "html5"
description: "html을 학습합니다."
---

# accesskey

```html
<script>

function foundItem() {

alert("found!!");

}

</script>

<body>

<a href="javascript: foundItem()" accesskey="n">foundItem</a>

</body>
```

accesskey 속성은 마우스 등을 쓰지 않는 환경을 위해 링크나 입력 폼에서 키보드의 키 입력만으로 동작을 실행할 수 있도록 accesskey 속성값에 access 할 영어 또는 숫자 한문자를 지정하여 단축키를 설정한다.

accesskey의 실행 방법은 사용자의 OS와 브라우저에 따라 다르다. 특히, 다른 브라우저와는 다르게 IE(인터넷 익스플로러)에서는 <a> 태그에 지정된 accesskey를 실행하면 지정된 링크가 실행되는 것이 아니라, <a> 태그로 포커스가 이동된다. 이때 Enter를 눌러야 지정된 링크가 실행된다.

IE(인터넷 익스플로러에서는 예약어(F, E, V, A, T, H)는 사용 할 수 없다.

* 브라우저별 accesskey 실행 방법

1. Window IE 6/7/8/9 : Alt + accesskey -> 포커스 이동

2. Window Firefox 3 : Alt + Shift + accesskey -> 실행

3. Window Safari 5 : Alt + accesskey -> 실행

4. Window Chrome : Alt + accesskey -> 실행

5. Window Opera 10 : Shift + Esc + accesskey -> 실행



출처: http://itmemo.tistory.com/124 [IT 지식 데이터베이스]