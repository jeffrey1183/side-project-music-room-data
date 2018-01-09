#The HTTP stands for HyperText Transfer Protocol

HyperText is text with links in it \(like [this](http://www.w3.org/)!\) and a transfer protocol is a fancy way of saying "rules for getting something from one place to another." In this case, the rules are for transferring web pages to your browser.

```js
var xhr = new XMLHttpRequest();
xhr.open("GET", "https://www.codecademy.com/", false);
xhr.send();

console.log(xhr.status);
console.log(xhr.statusText);
```

## The Client/Server Relationship

```
//////////
//Server//
//////////
// ////////// \\
// ////////// \\
// || \\
// // || \\ \\
////////// // || \\ //////////
//Client// // || \\ //Client//
////////// // || \\ //////////
////////// ////////// //////////
//Client// //Client// //Client//
////////// ////////// //////////
```

We can use HTTP to grab information from just about any web page on the Internet. But where do those web pages come from? They come from other computers on the Internet called **servers.**

The Internet is full of clients \(like your computer\) who ask for various resources \(web pages, files, and so on\), and servers, who store that information \(or know where to get it\).

When you make an HTTP **request**, it zips through the Internet until it finds the server that knows how to fulfill that request. Then the server sends a **response **back to you!

一台 server 可以一次處理很多 requests

## REST \(**Re**presentational **S**tate **T**ransfer\)

事實上 Client 和 Server 的觀念我們可以看作是一連串叫做 REST 的理論 \(**Re**presentational **S**tate **T**ransfer\)

* Remember how we said HTTP involves sending hypertext \(text with links\)? Whenever you navigate through a site by clicking links, you're making a **state transition** which brings you to the next page \(representing the next state of the application\). That's it!

* 其實道理很簡單就是 狀態的轉換，像點擊一個頁面的 button，跳到下一頁。

* 我們把有遵循這個規則的東西 稱作 RESTful

## A RESTful API

API 就像一種 coding contract

* It specifies the ways a program can interact with an application.

* 規範一個程式跟 app 的互動方式

* 舉例來說，如果你想要寫個 program 去讀取跟分析 twitter 的資料，你需要用 Twitter API，API 會 **specify the process for authentication, important URLs, classes, methods, and so on.**

### For an API or web service to be RESTful, it must do the following:

**對於 API 或是網站服務有這種 RESTful 的結構的話，就需要遵守下面三條規則**

* 把 Client 跟 Server 分開

* Not hold state between requests

* meaning that all the information necessary to respond to a request is available in each individual request; no data, or **state**, is held by the server from request to request\)

* 要使用 HTTP 和 HTTP methods，接下來會介紹


