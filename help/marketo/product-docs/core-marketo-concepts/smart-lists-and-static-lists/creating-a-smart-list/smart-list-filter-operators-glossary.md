---
unique-page-id: 557312
description: 智慧清單篩選器運算子字彙表 — Marketo檔案 — 產品檔案
title: 智慧清單篩選器運算子字彙表
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 1%

---

# 智慧清單篩選器運算子字彙表 {#smart-list-filter-operators-glossary}

運算子是智慧清單的一部分，可協助您取得特定資訊。 它可讓您以簡單明瞭的語言來描述您的篩選器或觸發器。 每種欄位類型的可用運算子都不同。

以下是描述每組運算子的辭匯表。

## 日期欄位 {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

選擇運算子時，右側會動態變更。

| 運算子 | 右側 | 說明 |
|---|---|---|
| is | 單一日期 | 完全符合日期 |
| 不是 | 單一日期 | 任何日期（指定的日期除外） |
| 介於 | 兩個日期欄位 | 包含和兩個指定日期之間的任何日期 |
| 過去 | 自然語言輸入&#42; | 請參閱下圖 |
| 以前 | 自然語言輸入&#42; | 請參閱下圖 |
| 未來 | 自然語言輸入&#42; | 請參閱下圖 |
| 以後 | 自然語言輸入&#42; | 請參閱下圖 |
| 時間範圍 | 預設集（上一季、昨天等） | 在選擇清單中定義 |
| after | 單一日期 | 指定日期之後的所有記錄 |
| befor | 單一日期 | 指定記錄之前的所有記錄 |
| 在或之後 | 單一日期 | 與&quot;after&quot;相同，但包含 |
| 在或之前 | 單一日期 | 與「之前」相同，但包容性 |
| 空白 | 無 | 沒有日期的所有記錄 |
| 非空白 | 無 | 具有任何日期的所有記錄 |

&#42; 自然語言輸入很酷。 您可以輸入以下一些模式：

* 1小時
* 82天
* 3週
* 14個月
* 1年

只要一起輸入號碼和單位，就行了！

>[!NOTE]
>
>&quot;過去&quot; **does** 納入您建立智慧清單的日期（直到時間，而非之後）。

>[!CAUTION]
>
>使用日期欄位篩選器（如出生日期、SFDC建立日期）建立智慧清單時，請使用 **befor** 或 **在或之前** 限制，智慧清單也包含在所述日期欄位中沒有值的人員。

請使用下圖來了解日期運算子之間的差異。

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**範例**
>
>處理過去和未來事件時，日期欄位可能會很棘手。 以下是幾個例子。
>
>**以前**
>
>對於您的新促銷活動，請使用此運算子，僅傳送電子郵件給未訂閱或已在一年內續訂服務，或從未訂閱的使用者。
>
>**以後**
>
>假設您想查看90天內有待續約的客戶。 您會使用兩個不同的篩選器。 首先使用「90天後」，然後使用「91天後」。 那會捕捉到90天後有約會的人。

## 字串欄位 {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| 運算子 | 說明 |
|---|---|
| is | 完全匹配（不區分大小寫） |
| 不是 | 除了完全匹配 |
| 開頭為 | 字串的前字母匹配 |
| 開頭為 | 字串的前幾個字母「不匹配」 |
| 包含 | 字串中的任何字母都匹配(範例：加利福尼亞，福特，為此) |
| 不包含 | 字串中沒有字母匹配。 （「包含」的反面） |
| 空白 | 沒有值的記錄(NULL) |
| 非空白 | 具有ANY值的記錄 |

>[!TIP]
>
>使用正運算子而非負運算子。 「不是」篩選器必須搜尋您例項中的整個資料集，這可能非常耗時。 正「is」篩選器可運用更有效的搜尋演算法。

## 整數欄位 {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">運算子</th> 
   <th colspan="1" rowspan="1">說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">完全數字匹配(= 0)將返回兩個帶有0的銷售機會 <em>和</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">不是</td> 
   <td colspan="1" rowspan="1">除了數字完全匹配</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">介於</td> 
   <td colspan="1" rowspan="1">定義兩個值，以找出介於兩者之間的每個人（包含）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">大於</td> 
   <td colspan="1" rowspan="1">高於指定</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">小於</td> 
   <td colspan="1" rowspan="1">小於指定</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">至少</td> 
   <td colspan="1" rowspan="1">高於指定（含）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">最多</td> 
   <td colspan="1" rowspan="1">小於指定（包括）</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">空白</td> 
   <td colspan="1" rowspan="1">沒有值(NULL)的記錄 — 零是數字，它是 <em>not</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">非空白</td> 
   <td colspan="1" rowspan="1">具有ANY值的記錄（包括零）</td> 
  </tr> 
 </tbody> 
</table>

如您所見，這些運算子讓您能輕鬆地說Marketo語！
