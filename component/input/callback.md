# Callback

```html
// callback="종류:함수명()"
// event: click, focus, keydown, input, keyup, enter, change, blur
// date evnet: select, selectMonth
<common-input callback="click:clickCallback()"></common-input>
```

```javascript

// @param val -> value
// @param fval -> dispaly text
// @param e -> {e:point event, comp:core component}

comp.clickCallback = function (val, fval, e) {}
comp.focusCallback = function (val, fval, e) {}
comp.keydownCallback = function (val, fval, e) {}
comp.inputCallback = function (val, fval, e) {}
comp.keyupCallback = function (val, fval, e) {}
comp.enterCallback = function (val, fval, e) {}
comp.changeCallback = function (val, fval, e) {}
comp.blurCallback = function (val, fval, e) {}

// type:date
comp.selectCallback = function (val, fval, e) {}
comp.selectMonthCallback = function (val, fval, e) {}
```
