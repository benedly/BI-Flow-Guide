# Callback

<pre class="language-html"><code class="lang-html"><strong>// callback="종류:함수명()"
</strong>// event: click, dblclick, check, selectRow, change, scroll, goToPage, changeRows
// date evnet: select, selectMonth
&#x3C;common-grid callback="click:clickCallback()">&#x3C;/common-grid>
</code></pre>

```javascript
// @param i -> tab index
// @param row -> row data
// @param col -> row column element
// @param key -> column field name
// @param e → {e: event, comp: component, row: row element}

// column click select
comp.clickCallback = function (i, row, key, e) {}

// column double click select
comp.dblclickCallback = function (i, row, key, e) {}

// row checkbox checked
// @param isCheck → row checked status 
comp.checkCallback = function (i, row, isCheck, e) {}

// row selection event
// @param isSelect → row select status
comp.selectRowCallback = function (i, row, isSelect, e) {}

// column data value change
comp.changeCallback = function (i, row, key) {}

// scroll stop event
// @param rows → body row numbers
comp.scrollCallback = function (startIdx, lastIdx, rows, e) {}

// page move event
comp.goToPageCallback = function (page) {}

// rows number changed after
comp.changeRowsCallback = function () {}

// Event after column render
comp.renderCallback = function (i, row, key, col) {}

// @param data -> grid data
// @param message -> grid no data message
comp.setDataCallback = function (data, message) {}

// footer render
comp.footerCallback = function (data, key) {
  // ex) if (key === 'age') return `<strong class="red"> ${data.sum(key)} </strong>`;
},

// footer summary render
comp.summaryCallback = function (data) {
  // ex) return `나이평균 <strong class="red"> ${data.avg('age').toFixed(1)} </strong>`;
},

// column sort
comp.sortCallback = function (key, order, type) {}

// Event after grid render
comp.completeCallback = function () {}
```
