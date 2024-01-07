# Option

### inlineText

```html
// form 형식이 아닌 value만 적용
<common-input option="inlineText"></common-input>
```

### theme

```html
// Set Component theme Class 
// default → "biflow-form-default"
<common-combo option="theme:default"></common-combo>
```

### cols

```html
// data value, text 설정
//[{VAL:1,TXT:'첫번재'},{VAL:2,TXT:'두번재'}]
<common-combo option="cols:VAL|TXT"></common-combo>
```

### format

```html
// 항목 text 영역 format
<common-combo option="format:#VAL# #TXT#"></common-combo>
```

### class

```markup
// Add Component Style Class 
// null(default), 'Class Name'
<common-combo option="class:Class Name"></common-combo>
```

### minWidth

```html
// The minimum width of the component. 
// '120px'(default), 'px'
const option = {minWidth: '120px'}
<common-combo option="minWidth:120px"></common-combo>
```

### width

```html
// null(default), 'px' or '%'
<common-combo option="width:300px"></common-combo>
```

### rows

```html
// The height of the scroll area. If it's a number, the number of rows.
// 8(default), 'px', number
const option = {rows: 8} 
<common-combo option="rows:10"></common-combo>
```

### label

```html
// null(default), 'label text'
<common-combo option="label:label text"></common-combo>
```

<div align="left">

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

</div>

### placeholder

```html
// null(default), 'placeholder text'
<common-combo option="placeholder:placeholder text"></common-combo>
```

<div align="left">

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

</div>

### _yyyyMM, yyyy, MM_

```html
// yyyyMM(년월), yyyy(년), MM(월)
// true, false(defulat)
// If it's true, range option is a must
<common-combo option="yyyyMM"></common-combo>
```

### number

```html
// true, false(default)
// If it's true, range option is a must. → range:'10~100' 
const option = {number: false} 
<common-combo option="number"></common-combo>
```

### range

```html
// 0 : today, current year, current month
// yyyyMM → '2000.1~2021.12'
// yyyy: → '2000~0'
// MM → -'3~0','all'(1~12)
// false(default), 'string'
<common-combo option="yyyy;range:2000~0"></common-combo>
```

### sort

```html
// 'asc'(default), 'desc'
// desc(내림차순), asc(올림차순)
<common-combo option="sort:desc"></common-combo>
```

### all

```html
// "전체" 항목 추가
// true, false(default)
<common-combo option="all"></common-combo>
```

### Component status

```html
<common-combo option="required"></common-combo>
```

| option   | Description          |
| -------- | -------------------- |
| required | false(default), true |
| disabled | false(default), true |
| readonly | false(default), true |

### tooltip

```html
// true(default), false
<common-combo option="tooltip:false"></common-combo>
```

### message

```html
// custom error message
// false(default), 'error message text'
<common-combo option="message:error message text"></common-combo>
```

### multiple

```html
// multiple select
// true, false(default), number(선택수제한)
<common-combo option="multiple"></common-combo>
```

### search

```html
// list search input field
// true, false(default)
<common-combo option="search"></common-combo>
```

### validate

```html
// Validation of "value" when focus is out
// true, false(default)
<common-combo option="multiple"></common-combo>
```
