---
description: templete <th option=""></th>
---

# Column Option

```javascript
option.column = "[headerName;dataField;width;...],...";
```

### width

```html
// column width
// '150px'(default), 'px', '%'
<th option="width:200px"></th>
```

### drag

```html
// Moving to Header Column Drag & Drop
// treu(default),  false
<th option="drag:false"></th>
```

### hide

```html
// column style display show/hide
// API hideCol & Api.showCol 연동
// true, false(default)
<th option="hide"></th>
```

### field

```html
// column data field & sort data field
<th option="field:null"></th>
```

### rowspan

```html
// Combining the same Column values
// true, false(default), 'data field'(field column dependent)
<th option="rowspan:true"></th>
```

### headerName

```html
// column header title
<th>header title</th>
```

### headerClass

```javascript
// Add header column class
// null(default), 'string'
<th option="headerClass:className"></th>
```

### headerAlign

```html
// header column text align
// 'center'(default), 'left', 'right'
<th option="headerAlign:left"></th>
```

### class

```javascript
// Add body column class
// null(default), 'string'
<th option="class:className"></th>
```

### ellipsis

```html
// column text 말줄임 사용여부 
// true(default), false
<th option="ellipsis:false"></th>
```

### align

```html
// body column text align
// null(default), 'left', 'center', 'ri
<th option="right"></th>
```

### valign

```html
// body column text virtical align
// null(default), 'top', 'bottom', 'middle'
<th option="top"></th>
```

### edit

```javascript
// column edit type
// true(input), false(default), 'input,combo,checkbox,radio'
<th option="edit:combo"></th>
```

### option

```html
// column edit 'input.combo' component option
// input & combo coponent 참조
<th option="edit:combo;option:'data:A600;cols:DETL_CD|DETL_CD_NM'"></th>
```

### resize

```html
// column resize
// true, false(default)
<th option="resize"></th>
```

### sort

```html
// column sort enable/disable & type
// true(type:text), false(default), 'number,date,text'
<th option="sort:false"></th>
```

### type

```html
// column type
// null(default), 'number', 'comma', 'fixed', 'date', 'textarea'
<th option="type:comma"></th>
```

### symbol

```html
// null(default), '₩', '₩,right'
// 99%
<th option="symbol:%,right"></th>
```

### mask

```javascript
// null(default), 'pattern,*타입','000###****,0',0(숫자),#(영문),*(숨김문자)
<th option="mask:000###****"></th>
```
