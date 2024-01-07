# API

### val

```javascript
// Get Value
comp.val();

// Set Value
comp.val('string');

// Set Date Value 
comp.val('20220131');
```

### fval

```javascript
// Get Display Value
comp.fval();
```

### setStyle

```javascript
// set html inline style css
comp.setStyle('width', '300px');
comp.setStyle('width:300px;pointer-events: none');
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
comp.required(); 
comp.required(true);

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

### cols

{% hint style="info" %}
type "checkbox, radio" only
{% endhint %}

```javascript
// Get Current cols
comp.cols();

// Set checkbox cols (checked value|unchecked value)
comp.cols("Y|N");

// Set radio cols (value^text|value^text)
comp.cols("Y^Yes|N^No")
```

### flush(target, idx)

{% hint style="info" %}
type "radio" only
{% endhint %}

```javascript
// @param target -> selector or object element
// @param idx -> cols index

// Move the all cols to the "#test1" element
comp.flush("#test1");

Move the cols[0] to the "#test1" element
comp.flush("#test1", 0);
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
