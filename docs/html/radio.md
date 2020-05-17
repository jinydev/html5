
#### radio : 
단일 선택자
클릭하면 선택할 수 있도록 합니다. 복수의 여러개의 선택이 있을 경우 하나만 선택할 수 있습니다.

여러개를 선택할때는 name 속성을 통하여 그룹화 시켜야 합니다.

```
<input type="radio" name="sex" value="남자"> 남자
<input type="radio" name="sex" value="여자"> 여자
```

동일한 name 값을 지정하게 되면, 선택된 하나의 결과값을 서버로 전송할 수 있습니다.