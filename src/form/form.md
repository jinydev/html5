---
layout: home
title: "html5"
keyword: "html5"
description: "html을 학습합니다."
---


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

