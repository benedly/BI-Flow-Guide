# API

## <mark style="color:blue;">DATA</mark>

### setData

```javascript
// @param data → data(json)
// @message → noData message
comp.setData(data, message); 
```

### getData

```javascript
// get all data
comp.getData();

// get row data 
// @rowIdx → row index number
comp.getData(rowIdx);
```

### noData

```javascript
// No Data 처리
comp.noData(message);
```

### addData

```
// Add Data
// @flag → scroll render
comp.addData(data, flag);
```

### clearData

```
comp.clearData();
```

### apply

```javascript
// 변경된 data 적용
comp.appy();
```

## <mark style="color:blue;">column</mark>

### addColDef

```javascript
// @colDef → '[headTitle;STATUS_NM;edit:combo;option:'data:STATUS_NM;cols:VAL|TXT'],..'
// @field → string(data field name)
comp.addColDef(colDef, field);
```

### setColData

```javascript
// @name → data name
// @data → data object(json)
// @flag → false(NOt redraw), undefined(redraw)
comp.setColData(name, data, flag)
```

### hideCol / showCol

```javascript
// @cols → column index or column field name
// (0,3) or ('name','age')
comp.hideCol(cols);
comp.showCol(cols);
```

### setHeader

```javascript
// header column innerHTML 
// @field → column define field name
// @label → text or html
comp.setHeader(field, label)
```

## <mark style="color:blue;">treeGrid</mark>

### expandAll

```javascript
// Spreading out the entire treeGrid.
comp.expandAll()
```

### expand

```javascript
// open the row(idx)
comp.expand(rowIdx)
```

### collapseAll

```javascript
// Folding the entire treeGrid.
comp.collapseAll()
```

### collapse

```javascript
// close the row(idx)
comp.collapse(rowIdx)
```

## <mark style="color:blue;">status</mark>

### updateRow

```javascript
// @flag → false(Nor redraw), undefined(redraw)
comp.updateRow(rowIdx, field, val, flag)
```

### updateCheck

```javascript
// row status 'update' check
// @flag → false(status ''), undefined(status 'update')
comp.updateCheck(rowIdx, flag)
```

### removeRow

```javascript
// if row status 'i' → remove row dom
// else → status 'd'
comp.removeRow(rowIdx)
```

### getTransactionData

```javascript
// if @status undefine → return all status(i,d,u) row data
// else → retern @status row data
comp.getTransactionData(status)
```

## <mark style="color:blue;">page</mark>

### setPage

```javascript
comp.setPage({
  // page: 2,
  // total: 1930,
  // pagination: 10,
  // rows: 100
})
```

### getPage

```javascript
// return {page: 2, total: 1930,pagination: 10,rows: 100}
comp.getPage()
```

### goToPage

```javascript
comp.goToPage(pageNum)
```

## <mark style="color:blue;">render</mark>

### reset

```javascript
// gird data reset & redraw
// @rowIdx → row dom data reset & redraw
comp.reset(rowIdx)
```

### redraw

```javascript
// gird redraw
// @rowIdx → row dom redraw
comp.redraw(rowIdx)
```

### setScroll

```javascript
// Set scroll postion
// x : number(%),  %, px
// y : number(rowIdx), %, px
comp.setScroll({x:val,y:val})
```

## <mark style="color:blue;">selection</mark>

### getSelectedIndex

```javascript
// return current selected row index
comp.getSelectedIndex();
```

### getSelectedData

```javascript
// return current selected row data
comp.getSelectedData();
```

### clearSelected

```javascript
// clear current selected row 
comp.setScroll();
```

### removeSelectedData

```javascript
// current selected row remove
comp.removeSelectedData();
```

## <mark style="color:blue;">checked</mark>

### setChecked

```javascript
// row checked
// @flag → checked value
comp.setChecked(rowIdx, flag);
```

### getCheckedIndex

```javascript
// return current Checked row index
comp.getCheckedIndex();
```

### getCheckedData

```javascript
// return current Checked row data
comp.getCheckedData();
```

### clearChecked

```javascript
// clear current Checked row 
comp.clearChecked();
```

### removeCheckedData

```javascript
// current Checked row remove
comp.removeCheckedData();
```

## <mark style="color:blue;">event</mark>

### formatter

```javascript
// columm option format
comp.formatter({
    formatter_name: function (i, row, key) {
        return '£' + row[key];
    },...
});
```

### render

```javascript
// columm render
comp.render(function (i, row, key) {
        return '£' + row[key];
    },...
});
```

## <mark style="color:blue;">etc</mark>

### meta

```javascript
// Developer temporary meta data management

// Get meta data
comp.meta();

// Reset meta data 
comp.meta('') or comp.meta('reset')

// Set meta data
comp.meta({title:text});
```
