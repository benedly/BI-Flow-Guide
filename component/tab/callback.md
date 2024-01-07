# Callback

```html
// callback="종류:함수명()"
// event: click, select
<common-tab callback="click:clickCallback()"></common-tab>
<div id="tab1">tab1</div>
```



```javascript
// @param i -> tab index
// @param tabTarget -> tab target dom
// @param e -> {id: "tab2", index:0, load: false, title: "title1"}
comp.clickCallback = function (i, e) {};
comp.selectCallback = function (i, tabTarget, e) {};
```
