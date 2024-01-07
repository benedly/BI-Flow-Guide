# type:date Option

### dateFormat

```html
// 'yyyy-MM-dd'(default)
<common-input option="type:date;dateFormat:yyyy-MM-dd"></common-input>
```

### dependency

```html
// The value depends on the "date component id" component
// null((default), 'date component id'
<common-input option="type:date;dependency:comp id"></common-input>
```

### disableDay

```html
// Not available on a specific day.
// 0~6 (일월화수목금토)
// null(default), [0,1], '0,1'
<common-input option="type:date;disableDay:0,1"></common-input>
```

### disableDate

```html
// Not available on a specific date.
// null(default), [20210101,20210408], '20210101,20210408'
<common-input option="type:date;disableDate:20210101,20210408"></common-input>
```

### disableRange

```html
// Not allowed to use a specific date and period.
// null(default), ['20210408~20210420', '12d~18d'] or '20210408~20210420,12d~18d'
<common-input option="type:date;disableRange:12d~18d"></common-input>
```
