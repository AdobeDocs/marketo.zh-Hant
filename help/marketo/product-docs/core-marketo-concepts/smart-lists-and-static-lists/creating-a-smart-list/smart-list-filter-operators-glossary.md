---
unique-page-id: 557312
description: 智慧型清單篩選器運算子辭彙表-Marketo檔案——產品檔案
title: 智慧清單過濾器運算子辭彙表
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 智慧清單過濾器運算子辭彙表{#smart-list-filter-operators-glossary}

運算子是智慧型清單的一部分，可協助您獲得特定資訊。 它可讓您以直接的語言來描述您的篩選或觸發。 每種欄位類型的可用運算子都不同。

以下是描述每組運算子的辭彙表。

## 日期欄位{#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

當您選擇運算子時，右側會動態變更。

| 運算元 | 右側 | 說明 |
|---|---|---|
| is | 單一日期 | 完全符合日期 |
| 不是 | 單一日期 | 任何日期（指定的日期除外） |
| wether | 兩個日期欄位 | 任何日期，包括兩個指定日期之間 |
| 過去 | 自然語言輸入* | 請參閱下圖 |
| 以前 | 自然語言輸入* | 請參閱下圖 |
| 未來 | 自然語言輸入* | 請參閱下圖 |
| 以後 | 自然語言輸入* | 請參閱下圖 |
| 在時間範圍內 | 預設集（上一季、昨天等） | 定義於挑選清單中 |
| after | 單一日期 | 指定日期後的所有記錄 |
| befor | 單一日期 | 指定之前的所有記錄 |
| on或after | 單一日期 | 與&quot;after&quot;相同，但包含 |
| on或之前 | 單一日期 | 與「之前」相同，但包含 |
| 空白 | 無 | 沒有日期的所有記錄 |
| 不為空 | 無 | 所有記錄及任何日期 |

*自然語言輸入很酷。 以下是您可以輸入的一些模式：

* 1小時
* 82天
* 3週
* 14個月
* 1年

只要一起輸入號碼和單位，就行了！

>[!NOTE]
>
>「過去」**does**&#x200B;包含您建立智慧型清單的日期（直到時間，而非之後）。

>[!CAUTION]
>
>當您使用日期欄位篩選器（如出生日期、SFDC建立日期）建立智慧清單，並在&#x200B;**之前或之前使用****約束時，智慧清單還將包括那些在該日期欄位中沒有值的人員。**

請使用下圖來瞭解日期運算子之間的差異。

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**範例**
>
>當您處理過去和未來事件時，日期欄位可能會變得棘手。 以下是幾個例子。
>
>**過去**
>
>若是您的新促銷活動，請使用此營運商僅傳送電子郵件給未在一年內訂閱或續約您服務或從未訂閱過服務的使用者。
>
>**以後**
>
>假設您想看到90天內有續約的客戶。 您應使用兩個不同的篩選條件。 首先使用「90天後在未來」，然後使用「91天後在未來」。 這可以捕捉到90天後有日期的人。

## 字串欄位{#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| 運算元 | 說明 |
|---|---|
| is | 完全符合（不區分大小寫） |
| 不是 | 除完全匹配外的任何內容 |
| 開始於 | 字串比對的首字母 |
| 開頭為 | 字串首字母DO NOTmatch |
| contains | 字串中的任何字母都符合(範例：加州，為此而財富) |
| 不包含 | 字串中沒有字母相符。 （「包含」的反面） |
| 空白 | 沒有值的記錄(NULL) |
| 不為空 | 具有ANY值的記錄 |

>[!TIP]
>
>使用正運算子而非負運算子。 「Is not」篩選器必須搜尋您例項中的整個資料集，這可能非常耗時。 正&quot;is&quot;篩選可運用更有效的搜尋演算法。

## 整數欄位{#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">運算元</th> 
   <th colspan="1" rowspan="1">說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">完全符合數字（= 0將返回兩個銷售線索，並且<em>和</em> NULL）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">不是</td> 
   <td colspan="1" rowspan="1">任何EXCEPT完全相符的數字</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">wether</td> 
   <td colspan="1" rowspan="1">定義兩個值，以找出介於兩者（含）之間的每個人</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">大於</td> 
   <td colspan="1" rowspan="1">在指定的</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">小於</td> 
   <td colspan="1" rowspan="1">小於指定的</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">至少</td> 
   <td colspan="1" rowspan="1">在指定（含）以上</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">最多</td> 
   <td colspan="1" rowspan="1">小於指定（含）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">空白</td> 
   <td colspan="1" rowspan="1">沒有值(NULL)-零是數字，它是<em>not</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">不為空</td> 
   <td colspan="1" rowspan="1">具有ANY值的記錄（包括零）</td> 
  </tr> 
 </tbody> 
</table>

如您所見，這些營運商讓Marketo話的流利性很好！
