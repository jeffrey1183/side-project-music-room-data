#Quiz: Data Types And Meaning
Here's another table. This one has some people's heights and weights in it. Each row of this table contains the same sort of data about a different person.
>我們來看另一個 table，這個 table 有不同人的身高與體重。

![](/assets/quizDataType_1.png)

As a programmer, we're familiar with the idea of data types. A string like Alan is a different type from a numerical value like 188. But 188 is the same type as 72 even though they present values with different meanings.One is the height in centimeters and the other is the weight in kilograms. Every column in the database table will have some type associated with it. All the values in that column will be of the same type. But, moreover, they also have the same kind of meaning. We wouldn't mix centimeters and kilograms in the same column.

>身為一個 programmer，我們對數字和字串很熟悉，然而 188 跟 72 雖然都是數字但他們是代表著不同意義，像中間這欄是身高，最右邊是體重。我們不能把這兩欄混在一起。

![](/assets/quizDataType_2.png)

The database system itself doesn't know which numbers are centimeters and which numbers are kilograms. We have to keep track of that for ourselves when we write code.
>資料庫本身不知道哪一欄的單位是身高，哪一欄的單位是體重，我們必須自己記得。


Here is another example. Georgia is a string, a piece of text. But a string that presents the name of country, like Georgia. Does not have the same kind of meaning as a string that represents a U.S. state, like Georgia, or the font of Georgia, or someone's first name, like Georgia O'Keeffe.
>另一個例子像是 Georgia 這個字串，他可能代表一個國家，也可能代表美國的喬治亞州，或是有一種字體也叫 Georgia，甚至是一個人的姓氏。

![](/assets/quizDataType_3.png)

To think about this more clearly, let's have a quiz. Here are five pieces of data. Check two pieces of data that definitely have the same type.
>練習一下，把兩個相同 data type 的選項勾起來。
![](/assets/quizDataType_4.png)

Yes! "Georgia" and "Ursus arctos" are both strings.
>"Georgia" 和 "Ursus arctos" 都是字串，413是 integer，(15,-5) 是座標，127.0.0.1 是 IP，有些系統可能當作數字拉，但也可能會有不同處理。
