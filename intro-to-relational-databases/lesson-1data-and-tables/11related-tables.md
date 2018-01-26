#Related Tables
A Database usually has several tables in it. Here's how we might start for our image voting app.
>資料庫通常會有很多 table，我們或許可以這樣開始我們的投票 App

![](/assets/relatedTables_1.png)

The first table presents pictures that people have uploaded of animals. The second presents people's votes.Fluffy, Master, George all are animals, whose pictures someone has uploaded. Because we might have two animals with the same names. We give each one numeric id here. The votes table says, which images have been displayed together for voting, and which one the user picked as the cutest. Here the app displayed Master the id 2, and George id 3 and the user voted for George. 2 and 3 were matched up and 3 was the winner. Note that in the vote table, the columns are called left,right and winner. But they matched up, to the column called id in the picture table. 
>左邊的 table 代表已經上傳的動物圖片，Fluffy, Master, George 都是已經上傳圖片的動物，為了怕有一樣的動物名，我們還設了 id 。右邊則是投票情形，圖片會並排呈現給用戶投票，讓用戶選擇哪一個比較可愛。像第一列就是指，左邊是 id 為 2 的 Monster，右邊是 id 為 3 的 George，結果用戶選了 George。右邊的三個欄位 left, right, winner 都跟 左邊的 id 欄位匹配。

![](/assets/relatedTables_2.png)

You can read every row as a sentence. In the pictures table, the sentences say Fluffy has id number 1 and the filename fluffsocute.jpg. Monster has the id number 2 and the filename monstie-basket.jpg and so forth. In votes table, the sentences are the picture 2 and picture 3, were displayed the user voted for picture 3 and so on. So the two 3 refer to the same thing, a cute critter in with id number 3. But they're in different tables and the columns have different names because they play different roles in different sentences. In left table, we're saying which picture has which id? In right table, we're saying which ones have been displayed together, and who got the vote?
>在 picture table 裡每一列其實都可可以當作一行句子，像第一行就是 Fluffy 的 id number 是 1，檔案名是 fluffsocute.jpg。在 votes table 裡第一行可以變成 圖2跟圖3，用戶選了圖3。左右邊的圖都有 3，他們指的是同一件事，一個id是3的可愛動物，但他們在不同 table，且 column 名稱不同，這表示他們在不同的「句子」扮演不同的角色。像左邊就是說哪一張圖對應哪一個 id，右邊就是，哪幾張圖並列，哪張圖得到用戶的青睞。
![](/assets/relatedTables_3.png)

So this is kind of sentence that the table actually represents. If you want to come up with some sentences like Monster was shown with Fluffy and Fluffy got the vote instead of 2 was shown with 1 and 1 got the vote. We would have to connect two tables.
>對於 vote 這個 table，如果我們想要顯示的是 Monster was shown...這樣的表示方式，而不是 2 was shown with.... 這種代數的方式，我們就要把兩個 table 連結在一起。
![](/assets/relatedTables_4.png)

That's something that we can do with a database query as well. Queries do this are called joins, we'll see a lot of them in later on in the course. For now we just remember that a value with the same meaning can occur in different table and have different column names and we can derive new tables by linking up existing tables with joins.
>要把兩個 table 我們可以用 join 這個 database query，我們會在接下來的課程一直用到。現在我們只要記得含義相同的一個值可以出現在不同 table 而且欄位的名稱還可以不同。我們可以用透過 join 把現有的 tale連在一起，得到新的 table
![](/assets/relatedTables_5.png)
