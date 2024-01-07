# Usage

### Javascript

```html
<span id="targetId"></span>
```

```javascript
/** 
 * @param compId -> 'string'
 * @param option -> 'string' or 'object'
 * @returns {*}
 */
const comp = biflow4.component.input(compId, option);
// const comp = biflow4.component.input(option);

// append dom
const targetEL = document.getElementById(targetId);
targetEL.appendChild(comp.$dom);

```

### Bootstrap

```html
<common-input id="compId" option="" callback=""></common-input>
```
