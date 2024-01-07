# Option

### type

```html
// hp(핸드폰), tel(일반전화), phone(전화 All)
// drive(운전면허번호)
// rNUm(주민번호), rrNum(내국인 주민번호), arNum(외국인 등록번호), crNum(사업저 등록번호)
<common-form type="hp"></common-form>
```

### inlineText

```html
// form 형식이 아닌 value만 적용
<common-form option="inlineText"></common-form>
```

### cols

```html
// form 각 구성요소 설정 
// input & combo option 사용
<common-form type="hp" cols="[width:50px][width:38px][width:85px]"></common-form>
```

### dash

{% code overflow="wrap" %}
```html
// '-' (default), false, string
<common-form type="hp" option="dash:, "></common-form>
<common-form type="hp" cols="[width:50px;dash:false][width:38px][width:85px]"></common-form>
```
{% endcode %}

### combo

```html
// type 'ht,tel, phone'일때 국번을 combo로 사용 
<common-form type="hp" combo></common-form>
```

### Component Status

{% code overflow="wrap" %}
```html
<common-form required></common-form>
```
{% endcode %}

| option   | Description                        |
| -------- | ---------------------------------- |
| required | all type                           |
| disabled | all type                           |
| readonly | input, date, textarea, search only |
