# スニペット

## 現在のページをTwitterにシェアするブックマークレット
参考: [[JavaScript][ブックマークレット] 現在のページをTwitterにシェアする用のブックマークレットを作成 - Qiita](https://qiita.com/koara-local/items/3e4bdcf1f929e619344c)
```javascript
javascript: (function () {window.open("https://twitter.com/intent/tweet?url=" + encodeURIComponent(location.href) + "&text=" + encodeURIComponent(document.title),"_blank", "width=600,height=300");})();
```