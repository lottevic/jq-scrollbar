# jQuery Scrollbar 範例

 [jQuery Scrollbar (官網)](https://gromo.github.io/jquery.scrollbar/) 是一個跨瀏覽器的通用scrollbar。
 ###  特色：
 * Browser support: IE7+, Edge, Firefox, Opera, Chrome, Safari
 * iOS 手機/平版也通用
 * 官網的demo並沒有做RWD範例，但實測是可以套用在iOS手機上，因iOS手機預設不顯示scrollbar，當某些網頁區塊需要顯示scrollbar時，就可以使用此套件!

> [jQuery Scrollbar 範例 @lottevic](https://lottevic.github.io/jq-scrollbar/src/)   
>  ![printscreen](images/qr-code.png)

##  Setting up
```html
  <!-- css -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/jquery.scrollbar/0.2.11/jquery.scrollbar.css" />
  <!-- jquery  -->
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
  <!-- jquery scrollbar -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery.scrollbar/0.2.11/jquery.scrollbar.min.js"></script>
```
##  套用 scrollbar-inner
![printscreen](images/01.png)
* html
```html
<div class="lotte-wrapper scrollbar-inner">
  <div class="lotte-article">
    <p> 依金管會規定...... </p>
  </div>
</div>
```
* js
```javascript
$( document ).ready(function() {
    $('.scrollbar-inner').scrollbar();
});
```
* css
```css
.lotte-wrapper{ //在自訂class中指定寬高
  max-width: 600px;
  width: 90%;
  height: 160px;
}
.lotte-article{ //padding設在下一層
  padding: 16px 16px 0 16px;
}
```
##  其他樣式： scrollbar-rail
![printscreen](images/02.png)
* html
```html
<div class="lotte-wrapper scrollbar-rail">
  <div class="lotte-article">
    <p> 上傳之資料...... </p>
  </div>
</div>
```
* js
```javascript
$( document ).ready(function() {
    $('.scrollbar-rail').scrollbar();
});
```
##  其他樣式： google chrome
 ![printscreen](images/03.png)
* html
```html
<div class="lotte-wrapper scrollbar-chrome">
  <div class="lotte-table">
    <table>...</table>
  </div>
</div>
```
* js
```javascript
$( document ).ready(function() {
    $('.scrollbar-chrome').scrollbar();
});