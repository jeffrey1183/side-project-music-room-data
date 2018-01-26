#How Queries Happen
Now we've seen some sort of information that we can store in a database table, let's talk about how our codes talks to a database. When our code fetches data out of a database, it does this by sending a query. In response, the database will send a result containing a new table with the data we ask for.
>現在我們來講講我們的程式碼是怎麼跟資料庫溝通的呢？我們是透過發送 query 到資料庫裡獲得資料，作為回應，database 會發一個新 table 其中包含我們要求的數據。

![](/assets/howQueryHappen_1.png)

Depending on the specifies of our environment our code might be talking to the database over the network.



Or it might just be calling the library that keeps the database on the local disk.

![](/assets/howQueriesHappen_2.png)

Those design details would be important later but for now we can actually ignore them. The basic of database work the same no matter what the implementation is. So let's take a look at running some queries in SQL against an actual database. Don't worry about this syntax right now, we'll see that in next lesson.
>資料庫的基本原理都是相同的，不論執行的是什麼操作，我們先來試著在資料庫裡跑 SQL，先不用擔心語法，下一節課會講到語法

Okay, here is the query we saw before, select food from diet where species equals orangutan.
>這是我們上一節提到的 query
![](/assets/howQueriesHappen_3.png)

And we run it here is the result. Now, something to notice about the result is that it's a table. It has two rows, it has one column, the food column that we asked for.
>跑完的結果就會像下面這樣，有兩列一欄，這一欄是我們要的關於食物的資料。
![](/assets/howQueriesHappen_4.png)

So running a query against the database isn't like returning a single value from a function, it's more like returning a list, even if there might only be one element.
>因此我們可以看出跑一個 query 跟跑 function 後回傳一個值不太一樣，而更像回傳一個列表，即使只有一個 element。

In fact, even if we ask the database for 2 plus 2 like this. The answer is still actually a table with one column and one row.
>如果我們輸入 2+2 到資料庫內，回傳的值一樣會是一個列表，包含一行和一列 。
![](/assets/howQueriesHappen_5.png)

If we ask the database for the answers to three arithmetic problems at once then we'll get back a table with a single row and three columns, each of them giving one of the answers.
>如果我們一次運算三個算式的話，回覆的 table 會有一列三欄，每一欄有自己的答案。
![](/assets/howQueriesHappen_6.png)

You might have noticed that these columns have rather unusual names, they all are question marks column question mark. If we want to give them more descriptive names, we can do that. By using as sum here, we get back still a table with one row and one column, but now the column has a more descriptive name of sum instead of question mark column question mark
>你可能已經注意到 ?column? 出現在欄位上，如果我們想要改變欄位名稱，我們可以在算式後面加上 as sum，table 就會出現 sum 的欄位名稱。
![](/assets/howQueriesHappen_7.png)

