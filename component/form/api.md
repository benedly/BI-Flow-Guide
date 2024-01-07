# API

### val

```javascript
// Get Value
comp.val();

// Set Value 
comp.val(val);
```

### fval

```javascript
// Get Display Value
comp.fval();
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

### inspect

```javascript
// 유효성 검사
// {result: true, value: "1234567890"}
// {result: false, type: "mask", value: "1234567890"}
// "type" is an error type when "result" is false.
comp.inspect();
```

### setLock

```javascript
// disable callback
comp.setLock(); 
comp.setLock(true);

// enalble callback
comp.setLock(false);
```
