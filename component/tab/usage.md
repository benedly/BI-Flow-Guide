# Usage

### Javascript

```html
<div id="targetId"></span>
```

```javascript
/** 
 * @param compId -> 'string'
 * @param option -> 'string' or 'object'
 * @returns {*}
 */
const option = "tabs:[tab1|title1][tab2|title2];select:0";
const comp = biflow4.component.tab(compId, option);
// const comp = biflow4.component.tab(option);

// append dom
const targetEL = document.getElementById(targetId);
targetEL.appendChild(comp.$dom);
```

### Bootstrap

```html
<common-tab id="compId" option="tabs:[tab1|title1][tab2|title2];select:0"
    callback=""></common-tab>
<div id="tab1">tab1</div>
<div id="tab2">tab2</div>
```
