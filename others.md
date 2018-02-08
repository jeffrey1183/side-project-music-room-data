#[三層式架構](http://www.softinbox.com/html/product_01.html)

##二層式架構
客戶-伺服器架構（client-server，或說兩層式架構、主從式架構）可以讓使用者透過網路從遠端拿到服務。通常在客戶端的主機上，會需要裝置客戶端軟體，執行這個軟體就可以從伺服器端的資料庫讀取或寫入資料。兩層式架構有些缺點，一是所有的營運邏輯(business logic)都放在客戶端軟體上，伺服器端通常只放資料庫。

##二層式架構的缺點
這種架構只要從客戶端軟體發動就可直接至資料庫存取資料，若有人模擬原客戶端軟體的動作，即可惡意操作資料庫，因此安全性不佳。二是這樣的設計使得客戶端和伺服器端的網路流量需求很高，在內部網路使用勉強可行，但當跨Internet使用時(例如分公司的員工連回總公司)頻寬的需求量太大。

##三層式架構
為了改善兩層式架構的缺點，出現了三層式架構，將兩層式架構中客戶端軟體從資料庫存取資料的動作拉回伺服器端來做，再加上一個介面讓客戶端用來操作伺服器提供的服務(應該就是後台)，現在這個介面通常 web 化，使用者用瀏覽器連上伺服器端的網頁伺服器來取得服務。

三層式架構的三層是哪三層呢？
1. 展示層(presentation)，或說使用者介面層，~~通常由網頁伺服器擔任~~現在的話還有 app 。
2. 營運邏輯層(business logic)，或說應用層、AP層，負責從資料庫取出資料，整合後傳遞給網頁伺服器供使用者使用；或是接收使用者輸入的資料，整合後寫進資料庫。

3. 第三層是資料層(data)，通常是SQL、Oracle、MySQL這類的資料庫。

![](/assets/CS_1.jpg)

三層式架構（Three-Tier）分為客戶端應用程式（Client Application）﹐應用程式伺服器（Application Server）及資料庫伺服器（RDBMS, Relational Database Management System）﹒各層作用如下: 客戶端應用程式 這是負責處理客戶端的使用者介面及資料的先前處理﹐比如說資料形態的确認等等工作﹒ 應用程式伺服器 這是介于資料庫和客戶端應用程式間負責將客戶端應用程式的需求回應給資料庫伺器﹐再將資料庫的資料傳給客戶端應用程式﹒ 資料庫伺服器 這就是資料庫啦﹐我們一般都是使用現有的資料庫伺服器﹐比如MS SQL SERVER; InterBase; Oracle等等﹒ 我們結合以上三個層次﹐舉個例子來講﹐餐廳的服務生的身份就可以看作是一個應用程式伺服器﹐他會幫您（客戶端應用程式）點菜﹐把您的需要記錄整理出來后﹐再送進廚房（資料庫伺服器）﹐等菜做完后﹐再負責從廚房（資料庫伺服器）拿出給您（客戶端應用程式）

# analogy KK \[əˋnælədʒɪ\]

* 相似，類似\[C\]\[（+between/to/with）\]
* Let's go back to the analogy of computer languages being like regular spoken languages.

[Program 和 Application 的差別](https://stackoverflow.com/questions/4431819/what-are-the-differences-between-a-program-and-an-application)

row,column

* 列\(台灣\),行\(大陸\)

[CI 不是系統，是流程](https://dotblogs.com.tw/hatelove/archive/2011/12/25/introducing-continuous-integration.aspx)


