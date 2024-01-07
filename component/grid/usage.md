# Usage

## Java Script

#### HTML

```html
<div id="targetId"></div>
```

#### Javascript

{% code overflow="wrap" %}
```javascript
// Grid Define
const option = {
  // Grid Option
  theme: 'default',
  fix: null,

  // Column 공통 정의, Column Option 참조
  columnDefault: {}
  
  // Column 정의 1. Array Object
  columnDefs: [
    {headerName: 'headerName', field: 'dataField', type: 'date'},...
  ]
  // Column 정의 2. String
  column: "[headerName;dataField;width;...],[종류;COL1;120px;...]..."
}

/** 
 * @param {string|undefined} compId
 * @param {object} option
 */
const gird = biflow4.component(string, option);

// append dom
const targetEL = document.getElementById(targetId);
targetEL.appendChild(comp.$dom);

// initialization
gird.init();
 

// define column types
option.type = {
  // typeName: column option,
  number: {align: 'right', sort: 'number', ....},
}

// define column formatter
option.formatter = {
  EURO: function (i, row, key) {
      return '£' + row[key];
  }
}


// callback
comp.event({
  click: function (i, row, key, e) {},
  dblclick: function (i, row, key, e) {},
  check: function (i, row, isCheck, e) {},
  change: function (i, row, key) {},
  scroll: function (start, end, lines, e) {},
  changeRows: function () {},
  render: function (i, row, key, col) {},
  footer: function (data, key) {},
  summary: function (data) {},
  complete: function () {}
})

// formatter
comp.formatter({
  medal: funtion(i, row, key) {
    let str = '';
    if(key === 'gold' ) str = 'gold: ';
    else if(key === 'silver' ) str = 'silver: ';
    else if(key === 'bronze' ) str = 'bronze: ';
    retrun str + row[key];
  }
});

// render
comp.render(sss, function() {
});
```
{% endcode %}

## Template

#### HTML

{% code overflow="wrap" %}
```html
<common-grid id="compId" data="" option="height:10;edit;" callback="complete:compIdComplete()">
    <table>
        <colgroup>
            <col width="150px">
            <col width="150px">
            <col width="150px">
        </colgroup>
        <thead>
        <tr>
            <th option="field:COL1;edit:fase">title1</th>
            <th option="field:COL2;edit:combo;option:'data:COL2DATA;cols:VAL|TXT'"">title2</th>
            <th option="field:COL3">title3</th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>#COL1#</td>
            <td>#COL2#</td>
            <td>#COL3#</td>
        </tr>
        </tbody>
    </table>
</common-grid>
```
{% endcode %}

#### Javascript

```javascript
biflwo.comboData = [
    {VAL: "1", TXT: "콤보1"},
    {VAL: "2", TXT: "콤보2"},
    {VAL: "3", TXT: "콤보3"},
    {VAL: "4", TXT: "해외법인"}
]

comp.compIdComplete = function () {
    biflow.compId.setColData('COL2DATA', biflow.comboData, false);
    return 'redraw';
};
```
