# API

### format

```javascript
// 항목 text 영역 format
comp.format("#VAL# #TXT#'); 
```

### render

```javascript
// 항목 text 영역 render
comp.render(function (row){ 
    return row.VAL +' '+ row.TXT + ' : render';
});
```

### getData

```
// Get component Data List
comp.getData(); // data Array
```

### setData

```
// Set Component Data List
// @param data -> Array
comp.setData(data);
```

### addData

```
// add Component Data List
comp.addData(data);
```

### show

```
// open combo list window
comp.show();
```

### hide

```javascript
// hide combo list window
comp.hide();
```

### select

```javascript
// Get current selected Data row object
// option 'multiple' => [object, object]
comp.select();
> {VAL: "1", TXT: "사업자종류 값 변경"}
```

### val

```javascript
// Get Value
comp.val();

// Set Value 
comp.val(val);
```

### text

```javascript
// Get list Inner Text
comp.text();
```

### valueByText , textByValue

```javascript
// Get values from text
comp.valueBytext('text');

// Get text from value
comp.textByVlaue('value');
```

### focus

```javascript
// Set focus
comp.focus(); 
comp.focus(true);

// remove focus
comp.focus(false);
```

### required

```javascript
// Set required
comp.required(); or comp.required(true);

// remove required
comp.required(false);
```

### readonly

{% hint style="info" %}
type "text, textarea, date" only
{% endhint %}

```javascript
// Set readonly
comp.readonly(); 
comp.readonly(true);

// remove readonly
comp.readonly(false);
```

### disabled

```javascript
// Set disabled
comp.disabled();
comp.disabled(true);

// remove disabled
comp.disabled(false);
```

### enable

```javascript
// Set enable (disabled(false))
comp.enable();
comp.enable(true);

// remove enable (disabled(true))
comp.enable(false);
```

### reset

```javascript
// Reset to initial option
comp.reset();
```

### option

```javascript
// Get Current Option
comp.option();

// Set modify Option
comp.option({name:value}); //ex:{class:'addClassname'}
```

### inspect

```javascript
// 유효성 검사
// {result: true, value: "1234567890"}
// {result: false, type: "mask", value: "1234567890"}
// "type" is an error type when "result" is false.
comp.inspect();
```

### meta

```javascript
// Developer temporary meta data management

// Get meta data
comp.meta();

// Reset meta data 
comp.meta('') or comp.meta('reset')

// Set meta data
comp.meta({title:text});
```

### setLock

```javascript
// disable callback
comp.setLock(); 
comp.setLock(true);

// enalble callback
comp.setLock(false);
```
