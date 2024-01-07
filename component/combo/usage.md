# Usage

### Javascript

```html
<span id="targetId"></span>
```

```javascript
/** 
 * @param compId -> 'string'
 * @param option -> 'string' or 'object'
 */
const comp = biflow4.component.combo(compId, option);
// const comp = biflow4.component.input(option);

// set data
const combo_data = [
  {VAL:'1',TXT:'text_1'}
  {VAL:'2',TXT:'text_2'}
  {VAL:'3',TXT:'text_3'}
]
comp.data(combo_data);

// append dom
const targetEL = document.getElementById(targetId);
targetEL.appendChild(comp.$dom);

```

### Bootstrap

```html
<common-combo id="compId" option="" callback=""></common-combo>
```
