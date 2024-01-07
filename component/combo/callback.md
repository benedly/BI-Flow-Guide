# Callback

```html
// callback="종류:함수명()"
// event: click, focus, change, select, setVal, render
<common-combo callback="click:clickCallback()"></common-combo>
```

```javascript
// @param val -> value
// @param text -> dispaly text
// @param e -> {e:point event, comp:core component}
// @param row -> {VAL:1,TXT:'title'}

comp.clickCallback = function (val, text, e){},
comp.focusCallback = function (val, text, e){},
comp.changeCallback = function (val, text, e){},
comp.selectCallback = function (val, text, e){},
comp.selValCallback = function (e){},
comp.renderCallback = function (row){},
```
