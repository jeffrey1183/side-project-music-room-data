# Make a Request

要用下面這個範例來講解

```js
var xhr = new XMLHttpRequest();
xhr.open("GET", "https://www.codecademy.com/", false);


xhr.send()
console.log(xhr.status)
console.log(xhr.statusText)
```

* 第一行
* `xhr`variable, which stands for **XML HTTP Request. **This is how we make an HTTP request!
* 第二行

* We make the actual request to Codecademy.com.

* 光第一和第二行不夠，我們其實還沒 send our request 所以我們需要 3~5行

* `console.log` `xhr.status`和 `xhr.statusText`

* status 就是像\(that was that "200" from before\)

* statusText 像 "OK"

## **四種 HTTP Verbs**

* GET: retrieves information from the specified source \(像我們上面這個例子\)

* POST: sends new information to the specified source.

* PUT: updates existing information of the specified source.

* DELETE: removes existing information from the specified source.

So when we sent our GET request to codecademy.com, we retrieved information. When you add to or update your blog, you're sending _**POST or PUT requests**_; when you delete a tweet, there goes a DELETE request.

## **HTTP request 的組成**

分成三個部分

1. Request line
1. Tells the server what kind of request is being sent \(GET, POST, etc.\) and what resource it's looking for;
2. Header
1. Sends the server additional information \(such as which client is making the request\)
3. Body
1. which can be empty \(as in a GET request\) or contain data \(if you're POSTing or PUTing information, that information is contained here\).

```js
POST /codecademy/learn-http HTTP/1.1
Host: www.codecademy.com
Content-Type: text/html; charset=UTF-8

Name=Eric&Age=26
```

上面這個就是一個典型的例子

Note the POST information in the request line, the header information below it, and the data to be POSTed at the bottom \(最後一行\)

## Endpoints

* Endpoints are API-defined locations where particular data are stored.
* Just as you'll GET a pair of pants from PantsWorld or you'll GET a bag of peanuts from PeanutHut.

* For instance, if you're using the API for a video hosting service, there might be endpoints for **the most popular videos**, the most recent videos, or videos belonging to a certain genre or category.

## **Authentication & API Keys**

### API 簡介

* 跟真實的鑰匙一樣：an API key grants you access to a particular API.

* An alphanumeric \(字母與數字符號構成的\) string used to identify you to an API

* 會認出使用者，追蹤使用情形和有沒有惡意使用

* keep track of how their service is used and prevent unauthorized or malicious activity.

* API keys 落落長

**API keys are often long alphanumeric strings，如下圖**

![](/assets/The Request_1.png)

### **OAuth的基本概念**

* 是一種 protocol

* Some APIs require authentication using a protocol called OAuth

* Redirected to a page asking for permission to link an application with your account, you've probably used OAuth.


