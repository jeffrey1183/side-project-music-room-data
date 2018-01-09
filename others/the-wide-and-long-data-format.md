連結：[http://www.theanalysisfactor.com/wide-and-long-data/](http://www.theanalysisfactor.com/wide-and-long-data/)

數據分析跟 data 的設定息息相關，如果你資料設錯，其實也不用想要分析。關於資料的設定我們可以分成 long data format 和 the wide data format.

### The Wide Format

其實就是一筆資料一列，新增項目在後面，像下面的圖，每一個 county 有四個時間點，1970 開始，每次增加 10 年，然後有二個變數，一個是 job，指的是一個國家的工作數字，然後有 3 個預測的變數：Land Area, Natural Amenity \(4=no and 3=Yes\), 和畢業人數佔總人口的比例 \( The proportion of the county population in that year that had graduated from college.\)

* A subject’s repeated responses will be in a single row, and each response is in a separate column.

![](/assets/The Wide and Long Data Format_1.png)

因為 land area 跟 amenity 不會因為時間而改變，所以都只有一行，其他的就會一欄一欄增加。

### The Long Format

在 long format 裡，每個時間點都會 response 一條，所以這個圖裡的每個國家都會有四列，就會這樣一條一條，但是不會像上面往寬的發展

![](/assets/The Wide and Long Data Format_2.png)



### 兩個 Format 的比較

不同的分析可能需要使不同的 Format

* Wide format is required for [MANOVA](http://www.theanalysisfactor.com/repeated-measures-approaches/) and [repeated measures](http://www.theanalysisfactor.com/?s=repeated+measures) procedures.

* [mixed models](http://www.theanalysisfactor.com/concepts-you-need-to-understand-to-run-a-mixed-or-multilevel-model/) and many [survival analysis](http://www.theanalysisfactor.com/survival-analysis-webinar/) procedures require data to be in the long format.

* long format 就可以拿同一年的資料去比較

* 這兩種 format 之間的轉換可以用 Proc Transpose in SAS 或是 the Restructure wizard in SPSS.


