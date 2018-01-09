
* 官方網站：[http://getbootstrap.com/](https://www.gitbook.com/book/jeffrey1183/codecademy-notes/edit#)

* 手機網頁的前端架構

* 用於開發網站 Responsive 功能

## Grid System

Bootstrap comes with a grid that is made up of 12 equal-sized columns. HTML elements are arranged to span different numbers of columns in order to create custom page layouts.

> 用於排版，在Bootstrap是由12個相同的長條排列，長條上可以擺放HTML elements，排出你要的版型

![](https://lh4.googleusercontent.com/t_anBxLb0k6FOJnLL_W1EEtKRLaWybApoYENrvTSS-cKHy_RvIkPlxU0H2k9RZjpuHn32NSyfz4E6w7aGhil0UonC9FfQiDlgAfr15L-Kv6Sucmmp-s97BP5RBHjO6JDCGW7zYab)![](https://lh6.googleusercontent.com/U8jtNQGXPmJshlryJdZuHOAUUogasM96pYXtSPPddcOKZBBDtORDgG575n8uCOTnnKUVihOajn7Pk3g-7g6wEuiAksoUdeMWJYLlHiD7iayXSV5JeDz4FRKTByMWIvJcQkcyGCTD)

css 寫法 \(Medium devices Desktops\)

* 細節：[https://getbootstrap.com/docs/3.3/css/\#](https://getbootstrap.com/docs/3.3/css/#grid)grid

* 每一個單位為col-md-1，一個頁面總有col-md-12長

```css
<div class="row">
<div class="col-md-8">
<h4>Content 1</h4>

</div>
<div class="col-md-4">
<h4>Content 2</h4>
</div>
</div>
```

## Bootstrap 的 tab 語法

1.設定 ul 的 class 為"nav nav-tabs"

2.將要打開的 tab 設置 class 為 &lt;li class="active"&gt;

```css
<ul class="nav nav-tabs">
<li><a href="#">Primary</a></li>
<li><a href="#">Social</a></li>
<li><a href="#">Promotions</a></li>
<li class="active"><a href="#">Updates</a></li>
</ul>
```

* 實際操作可以到[這邊](https://www.w3schools.com/bootstrap/bootstrap_tabs_pills.asp)

## Bootstrap 的 pills 語法

1.設定ul的class為"nav nav-pills"

2.將要打開的tab設置class為&lt;li class="active"&gt;

```css
<ul class="nav nav-pills">
<li><a href="#">Primary</a></li>
<li class="active"><a href="#">Social</a></li>
<li><a href="#">Promotions</a></li>
<li><a href="#">Updates</a></li>
</ul>
```

* 實際操作可以到[這邊](https://www.w3schools.com/bootstrap/bootstrap_tabs_pills.asp)

## Jumbotron

* [說明](https://www.w3schools.com/bootstrap/bootstrap_jumbotron_header.asp)

## Jumbotron 案例

* 案例
* [http://www.apple.com/ios/](http://www.apple.com/ios/)
* [http://www.google.com/mobile/](http://www.google.com/mobile/)

```html
<div class="jumbotron">
<h1>Find a place to stay.</h1>
<p>Rent from people in over 34,000 cities and 192 countries.</p>
</div>
```

## 在 Html 內設定連結到 bootstrap.css檔案

&lt;link rel="stylesheet" href="[http://s3.amazonaws.com/codecademy-content/courses/ltp/css/bootstrap.css](http://s3.amazonaws.com/codecademy-content/courses/ltp/css/bootstrap.css)"&gt;

## 瀏覽器解讀 link tags的順序

```html
<head>
<link href="shift.css" rel="stylesheet">
<link rel="stylesheet" href="bootstrap.css">
<link rel="stylesheet" href="main.css">
</head>
```

瀏覽器解讀下列 link tags 中的優先讀取順序，最重要的是最下方的main.css

1.shift.css

2.bootstrap.css, and applies those styles to the page.

3.main.css, and applies those custom styles to the page. The custom styles override\(推翻\) the Bootstrap styles.

The order of the CSS files tell the browser that your styles in main.css are more important than the styles in bootstrap.css, so the final page that loads is the customized web page.


