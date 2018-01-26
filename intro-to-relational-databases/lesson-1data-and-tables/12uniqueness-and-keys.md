#Uniqueness And Keys
In a lot of databases, we're talking about unique entities out in the world. Like individual people or locations, or email accounts. If something is unique, there can't be two of them. So for instance, names are not unique, not even full names. There are a lot of people in the world named Jennifer Smith. But a particular person named Jennifer Smith is still a unique individual. You wouldn't want to give one person another person's grade or their parking tickets just because they share the same name. Whenever we want to ambiguously relate a row of one table to a row of another, to see they are about the same person or thing out in the world. We need to have a unique value to talk about that thing.
>在資料庫裡我們要處理很多唯一存在的東西，比如人、地點或是電子郵件。如果某樣東西是唯一的，那就不會有兩個，就像名字，世界上雖然有很多 Jennifer Smith，但每一個名叫 Jennifer Smith 的人都是獨一無二的個體，不會因為兩個人名字一樣，你的考試成績或是罰單就給了另一個人。如果我們要讓 table 有關聯，一定要確認內容指的是同一個人或同一樣東西，那個東西必須有唯一值。

In the cutest animal databases, we used a numerical ID for each animal picture, which we used to relate the votes table to it. That's pretty common choice. Just make up the unique number for your database. It's so common that most database system can do it for you. User IDs, comment IDs on forums and so on, are all examples of this.
>在可愛動物的資料庫裡，我們對每張動物的照片使用數字 ID，用這個 ID 跟投票的 table 進行關聯，在大多數的資料庫系統中相當常見，設一個唯一的數字。論壇上的 User ID、comment ID 都是這樣的例子。
![](/assets/unique_1.png)

In database terminology, a column and a table that uniquely identifies rows on that table, can be called the primary key.
>下面這張圖裡綠色的部分是唯一值，幫助我們辨別每一列，在資料庫的術語中，稱作 primary key。
![](/assets/unique_2.png)


Sometimes the world gives us a natural primary key for a table. For instance, you have a table of countries and their capital cities. You can be confident that there aren't two countries named France. So in that case, you can safely use the name of country as a key. You don't have to call it country number 29. But you have to make sure that a key really is unique.
>生活中就有些 primary key 的例子可以參考，像是如果你有一個國家名和首都的對應表，你可以確定世界上沒有第二國家也叫法國。在這種情況下，你可以放心用國家名當作 primary key，不用命名成第29個國家之類的。

![](/assets/unique_3.png)

For instance in the US, there are several states with a city named Springfield. There's Springfield Massachusetts, Springfield Illinois, and a whole bunch of others. So It's obvious that the name of Springfield isn't unique by itself. Now you might tempted to think that city plus state is unique, but it turns out that's not true either.

![](/assets/unique_4.png)