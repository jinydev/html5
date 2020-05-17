## picture
html5 에서 새롭게 등장한 요소입니다. 모바일 환경에서 사용하면 좋습니다.


```html
<picture>
    <source medai="(min-width:800px)" srcset="img1.png">
    <source medai="(min-width:400px)" srcset="img2.png">
    <img src="img3.png" alt="" style="width:auto">
</picture>
```

`미디어 크기`에 따라 다르게 이미지를 반응합니다.

방응형 웹에서 이미지를 달리 표현할 수 있습니다.