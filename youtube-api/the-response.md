# **The HTTP response structure**

mirrors that of the HTTP request. It contains:

* A response line

* A header

* The body

## HTTP Status Codes

一個成功 request to server 會產生一個 response, which is the message the server sends back to you, the client.

* 有時候會看到錯誤代碼 502 ，這個代碼叫做HTTP Status Codes

* 開頭從1xx,2xx,3xx,4xx,5xx，這個規定是[IETF](https://en.wikipedia.org/wiki/IETF)

* 各個代碼的簡介

* 1xx: You won't see these a lot. The server is saying, "Got it! I'm working on your request."

* 2xx: These mean "okay!" The server sends these when it's successfully responding to your request.

* 3xx: These mean "I can do what you want, but I have to do something else first." You might see this if a website has changed addresses and you're using the old one; the server might have to reroute the request before it can get you the resource you asked for.

* 4xx: These mean you probably made a mistake. The most famous is "404," meaning "file not found": you asked for a resource or web page that doesn't exist.

* 5xx: These mean the server goofed up and can't successfully respond to your request.

* Full List :[https://en.wikipedia.org/wiki/List\_of\_HTTP\_status\_codes](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes)

## Anatomy of a Response

The HTTP response structure mirrors that of the HTTP request. It contains:

1. A response line, which includes the three-digit HTTP status code;

2. A header, which includes further information about the server and its response;

3. The body, which contains the text of the response.

## XML是什麼？Parsing XML

* XML \(which stands for ExtensibleMarkupLanguage\)

* 很像 HTML ，使用標籤語言—it uses tags between angle brackets

* 差別在自創：XML allows you to use tags that you make up, rather than tags that the [W3C](http://www.w3.org/) decided on

For instance, you could create an API that returns information about a [pet](https://www.codecademy.com/courses/javascript-beginner-en-EID4t/2/3?curriculum_id=50ecb8d45f787a6332000042)：

```
<pet>
<name>Jeffrey</name>
<species>Giraffe</species>
</pet>
```

* As long as you document the structure of your API's response, other people can use your API to get information about &lt;pet&gt;s.

**
**

## **JSON 是什麼？Parsing JSON**

* JSON \(which stands forJavaScriptObjectNotation\) is an alternative to XML

* Data format 像 JavaScript objects

* 比 XML 簡潔\(succinct\)** ，**以下面這個&lt;pet&gt; 為例



```js
{
"pets": {
"name": "Jeffrey",
"species": "Giraffe"
}
}

```



## XML or JSON?

要怎麼知道 API will reply with XML or JSON? 就看 API 文件吧!!


