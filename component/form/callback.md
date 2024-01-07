# Callback

<pre class="language-html"><code class="lang-html"><strong>// callback="종류:함수명()"
</strong>// event: click, focus, change, select, keydown, input, keyup, blur, setVal
&#x3C;common-form callback="click:clickCallback()">&#x3C;/common-form>
</code></pre>

```javascript
// @param val -> value
// @param fval -> dispaly text
// @param e -> {e:point event, comp:core components}

comp.clickCallback = function (val, fval, e) {}
comp.focusCallback = function (val, fval, e) {}
comp.changeCallback = function (val, fval, e) {}
comp.selectCallback = function (val, fval, e) {}
comp.enterCallback = function (val, fval, e) {}
comp.keydownCallback = function (val, fval, e) {}
comp.inputCallback = function (val, fval, e) {}
comp.keyupCallback = function (val, fval, e) {}
comp.blurCallback = function (val, fval, e) {}
comp.setValCallback = function (e) {}
```
