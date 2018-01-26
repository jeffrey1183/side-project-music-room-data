#Aggregations
So in the last quiz, we saw one example of an aggregation, a database's operation of summarize multiple rows into a single row. Counting up the number of gorillas in the animals table was a count aggregation. It takes a several rows, each represents one gorilla and representing the count.This picture shows the results of a count aggregation on the animals table. It's a count aggregation, grouping the values in the table using the species column. In other words, it's counting the number of rows that have the same value in that column.

>上一個測驗中我們看到 aggregation 的一個例子，把很多行列的資訊彙整成單獨一列。數有幾隻大猩猩這種方式叫做 count aggregation，有幾行就代表有幾隻大猩猩。下面這張圖就把每一種物種有幾隻算了出來。


![](/assets/aggregation_1.png)


Any time we want to compute a single result from a set of values, that's an aggregation.
>每次我們想從一堆數據裡計算出單一個結果就叫做 aggregation。

Here are some of the most common aggregation functions in SQL. Count is different from the other ones, in that it takes value of any type, and returns a number. Most of the other aggregations only work on numbers. For instance, you can't average a column of string values because only numbers have an average.
>這張表是一些常用的 aggregation，count 跟其他 aggregation 不太一樣，他可以對任何資料類型的值做執行，算出一個數字，其他 aggregation 都只對數字做計算，就像你不能算出一堆字串的平均數。

![](/assets/aggregation_2.png)
