# Grid Option

### theme

```html
// Set Component theme Class 
// default → "biflow-form-default"
<common-grid option="theme:default"></common-grid>
```

### class

```html
// Add Component Style Class 
// null(default), 'Class Name'
<common-grid option="class:Class Name"></common-grid>
```

### noData

```html
// Message when I don't have data.
// '데이터가 존재하지 않습니다'(default), 'string text'
<common-grid option="noData:'데이터가 존재하지 않습니다'"></common-grid>
```

### rows

```html
// Number of pages row
// 50(default), Number
<common-grid option="rows:30"></common-grid>
```

### page

```html
// pagination page number
// 10(default) , number, false(scroll render)
<common-grid option="page:5"></common-grid>
```

### **pageTotalText**

```html
// pagination "total" text
<common-grid option="pageTotalText:'대상건수'"></common-grid>
```

### **pageRowsText**

```html
// pagination view setting text
<common-grid option="pageRowsText:'보기설정'"></common-grid>
```

### setRows

```javascript
// set slect row list
// '20,50,100'(default) , number,
<common-grid option="setRows:20,50,100"></common-grid>
```

### **rows**

```html
// display row number
// 50(default) , number,
<common-grid option="rows:20"></common-grid>
```

### width

```html
// '100%'(default), 'px' or '%'
<common-grid option="width:200px"></common-grid>
```

### autoWidth

```html
// Automatic setting of column width.
// true, false(default)
<common-grid option="autoWidth"></common-grid>
```

### height

```html
// '100%'(default), 'px', number(rows), 'auto'
<common-grid option="height:10"></common-grid>
```

### rowHeight

```html
// row element height of Body
// 30(default, px)
<common-grid option="rowHeight:30"></common-grid>
```

### headerRowHeight

```html
// row element height (px) of Header
// 30(default, px)
<common-grid option="headerRowHeight:30"></common-grid>
```

### rowAutoHeight

```html
// true, false(default)
// colum의 높이에 따라 자동으로 각각의 row height 값 설정
<common-grid option="rowAutoHeight"></common-grid>
```

### rowspan

```html
// Combining the same Column values.
// false, number(index) ex) 1,4^1,6^1   4^1(1열 기준)
<common-grid option="rowspan:1,4^1,6^1"></common-grid>
```

### indicator

```html
// Displaying the rows number
// true(virtual idx), false(default), 'idx'(data 고유 idx), 'string'(data field)
<common-grid option="indicator:false"></common-grid>
```

### status

```html
// Displaying the rows data status icon.
// true, false(default)
<common-grid option="status:false"></common-grid>
```

### check

```html
// Displaying the row checkbox
// true(multi checked), false(default), 'single'
<common-grid option="check:false"></common-grid>
```

### selectCol

```html
// column slection
<common-grid option="selectCol:false"></common-grid>
```

### selectRow

```html
// row selection
// true('single' default), false, 'multi'
<common-grid option="selectRow:false"></common-grid>
```

### fix, fixRight

```html
// 틀고정
// null(default), order number '1,2,3'  [1,2,3]
// order number → column index
<common-grid option="fix:0,1,2"></common-grid>
```

### lock

```html
// all column disable edit
// true, false(default)
<common-grid option="lock"></common-grid>
```

### editClick

```html
// 'dblclick'(default), 'click'
<common-grid option="editClick:dblclick"></common-grid>
```

### type

```javascript
// Define column type option
// null(default), object
// 'number,comma,fixed,date' 사전 정의됨
const option = {type: {
    type1: {
        sort: 'number'
        , align: 'right'
    },...
}}
```

### formatter

```javascript
// Define column formatter
// null(default), object
const option = {formatter: {
  EURO: function (i, row, key) {
    return '£' + row[key];
  },...
}}
```

### <mark style="color:blue;">Define basic options for columns</mark>

{% hint style="info" %}
'resize', 'sort', 'edit', 'option(edit option)', 'headerClass', 'headerAlign', 'align', 'valign', 'symbol', drag'
{% endhint %}
