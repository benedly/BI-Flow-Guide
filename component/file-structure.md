---
description: /src/main//webapp/static/framework
---

# File Structure

* **Framework**
  * <mark style="color:red;">**angular14**</mark>** :** Wrapping Core JS to Angular
    * <mark style="color:blue;">**directive**</mark>
      * CommonAuthDirective.js : 유저 권한(결재)정보&#x20;
    * <mark style="color:blue;">**service**</mark>
      * MenuNavigator.js
      * SessionManager.js
    * <mark style="background-color:orange;">**biflow4-angular.js**</mark>  : JS Core Angular Wrapping & Angular Component Build &#x20;
      * <mark style="color:blue;">**controller**</mark>
        * AbstractController.js
      * <mark style="color:blue;">**directive**</mark>
        * AbstractDirective.js
        * CommonChartDirective.js
        * CommonCodeDirective.js
        * CommonComboDirective.js
        * CommonDateDirective.js
        * CommonFormDirective.js
        * CommonGridDirective.js
        * CommonInputDirective.js
        * CommonLangDirective.js
        * CommonPopupDirective.js
        * CommonTabDirective.js
        * CommonTransactionDirective.js
        * CommonTreeDirective.js
        * CommonUploaderDirective.js
      * init.js&#x20;
  * <mark style="color:red;">**core**</mark>
    * <mark style="color:blue;">**fonts**</mark>
      * bootstrap-icons.woff
      * bootstrap-icons.woff2
    * <mark style="background-color:orange;">**biflow4.js**</mark>  : JS Core Component Build &#x20;
      * <mark style="color:blue;">**asset**</mark>
        * [ace](https://ace.c9.io/) : web editor
        * [chart.js](https://www.chartjs.org/) : chart
      * <mark style="color:blue;">**js**</mark>
        * <mark style="color:blue;">**components**</mark>
          * calendar.js : datepicker & calendar
          * chart.js : chart.js 연동
          * combo.js
          * dialog.js
          * echart.js : echart 연동
          * file-uploader.js
          * grid.js
          * input.js
          * popup.js
          * simple-tree.js
          * tab.js
        * <mark style="color:blue;">**system**</mark>
          * binder.js
          * bootstrap.js <mark style="color:blue;">- Html Custom Tag Component</mark>
          * lang-pack.js
          * spa-router.js
          * transaction.js
          * wss-connector.js
        * biflow.pkg.js : core 설정
        * GlobalJS.js&#x20;
        * system.js
      * <mark style="color:blue;">**scss**</mark>
        * common.css
        * component.css
        * root.css
        * style.css
    * **biflow4.css**
    * **layout\_\*.css** : Project Layout
    * **biflow4.config.js :**  Project biflow 환경설정
