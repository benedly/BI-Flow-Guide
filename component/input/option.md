# Option

### inlineText

```html
// form 형식이 아닌 value만 적용
<common-input option="inlineText"></common-input>
```

### type

```html
// Set Input Component Type
// text(default), password, textarea, date, radio, checkbox
<common-input option="type:text"></common-input>
```

### theme

```html
// Set Component theme Class 
// default → "biflow-form-default"
<common-input option="theme:default"></common-input>
```

### class

```html
// Add Component Style Class 
// null(default), 'Class Name'
<common-input option="class:Class Name"></common-input>
```

### minWidth

```html
// The minimum width of the component. 
// '120px'(default), 'px'
<common-input option="minWidth:120px"></common-input>
```

### width

```html
// null(default), 'px' or '%'
<common-input option="width:300px"></common-input>
```

### text align&#x20;

```html
// Components text alignment.
// left(default), right, center
<common-input option="right"></common-input>
```

### label

{% hint style="info" %}
type "checkbox" ( ![](<../../.gitbook/assets/image (9).png>) )

type "text, password, textarea, date, search" ( ![](<../../.gitbook/assets/image (10).png>) )
{% endhint %}

```html
//  null(default), 'label text'
<common-input option="label:label text"></common-input>
```

### placeholder

{% hint style="info" %}
type "text, password, textarea, search" only   ![](<../../.gitbook/assets/image (11).png>)
{% endhint %}

```html
// null(default), 'placeholder text'
<common-input option="placeholder:placeholder text"></common-input>
```

### Text Restrictions

{% code overflow="wrap" %}
```html
// 문자 입력제한
<common-input option="number:true;comma:true;fixed:2;regexp:num|kor|eng|\s"></common-input>
```
{% endcode %}

| option | value                       | description                             |
| ------ | --------------------------- | --------------------------------------- |
| number | true                        | 100000000                               |
| comma  | true                        | 100,000,000                             |
| fixed  | true                        | 100000000.12345...                      |
|        | 2(Number of decimal places) | 100000000.12                            |
| regexp | num                         | 0-9                                     |
|        | kor                         | ㄱ-ㅎㅏ-ㅣ가-힇                               |
|        | eng                         | a-zA-Z                                  |
|        | \*                          | {}\[]/?.,;:\|)\*\~\`!^-\_+<>@#$%&\\=('" |
|        | num\|kor\|eng\|\*\|-\_\s!@  |                                         |

### Component Status

{% code overflow="wrap" %}
```html
<common-input option="required"></common-input>
```
{% endcode %}

| option   | Description                        |
| -------- | ---------------------------------- |
| required | all type                           |
| disabled | all type                           |
| readonly | input, date, textarea, search only |

### val

```html
// ''(text default), false(radio, checkbox default)
<common-input option="val:value"></common-input>
```

### cols

{% hint style="info" %}
type "checkbox, radio" only\
![](<../../.gitbook/assets/image (12).png>)   ![](<../../.gitbook/assets/image (14).png>)
{% endhint %}

```html
// type:checkbox -> "Y|N" (checked value| unchecked value) 
// type:radio -> "Y^Yes|N^No" (value^text|value^text) 
<common-input option="type:checkbox;cols:Y|N"></common-input>
<common-input option="type:radio;cols:Y^Yes|N^No"></common-input>
```

### range, min, max

```html
// range: "string", min: "string", max: "string" 
// type "text" → component character "number, comma, fixed" -> range: -100~100
// type "date" → range:20000101~20211231, range:-1m~0 (y,m,d)
// null(default)
<common-input option="type:text;range:-10~10"></common-input>
<common-input option="type:date:range:~0"></common-input>
```

### length, minlength, maxlength

```html
// component character length
// length: "8~16", minlength: "8", maxlength: "16"
// null(default)
<common-input option="length:8~16"></common-input>
```

### mask

```html
// mask: "pattern, * "
// @pattern: 000-###-abc-00** (0: number, #: alphabet, *: hidden character)
// @*(hidden character): 0 or #
// false(default)
<common-input option="mask:000000-0******"></common-input>
```

### pattern

```markup
// phone (전화 All), hp (핸드폰), tel(일반전화)
// rNum (주민번호), rrNum (내국인 주민번호), arNum (외국인 등록증), crNum (사업자번호)
<common-input option="rNum"></common-input>
```

### symbol

```html
// 'text' or 'text, align' or [text, align] (default:false)
// @text: $,₩,€,£,¥....
// @align: left(default), right
<common-input option="symbol:%,right"></common-input>
```

<div align="left">

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

</div>

### tooltip

```html
// true(default), false
<common-input option="tooltip:false"></common-input>
```

<div align="left">

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

</div>

### message

```html
// custom error message
// false(default), 'error message text'
<common-input option="message:error message text"></common-input>
```

<div align="left">

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

</div>

### focusEnd

{% hint style="info" %}
type "text, textarea, search" only. ![](<../../.gitbook/assets/image (8).png>)
{% endhint %}

```html
// Position the cursor at the end of focus
// true, false(default)
<common-input option="focusEnd:true"></common-input>
```
