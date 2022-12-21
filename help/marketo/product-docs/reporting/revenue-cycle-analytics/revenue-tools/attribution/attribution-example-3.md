---
unique-page-id: 7514149
description: 歸因範例3 - Marketo檔案 — 產品檔案
title: 歸因範例3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# 歸因範例3 {#attribution-example}

請閱讀以下案例，並嘗試確定網格中應包含的數字。

* 4月11日 | Steve下載（內容） — 成功
* 4月22日 |為3,000美元（Steve和Jason都有角色）而建立的Opportunity
* 4月25日 | Jason到期（網路研討會） — 成功
* 4月30日 |機會是封閉的

| 歸因量度 | (內容) | （網路研討會） |
|---|---|---|
| (MT)已建立Opty | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT)管道已建立 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT)奧蒂元 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)收入成本 | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**顯示答案**

>[!NOTE]
>
>**說明**
>
>記住歸因規則#3。 建立後，Jason獲得了程式成功。 因此，網路研討會無法獲得機會創造的評分。 只有奧普蒂贏了。
>
>因此，（內容）對於建立和管道奧地利有100%的評分，但對於奧地利勝出只有50%的評分。

>[!NOTE]
>
>**歸因規則**
>
>1. 貸項均分
>1. 你不能比掙的多給
>1. 你不能因為過去發生的事而評價


請試用所有範例，您就會成為歸因專家！

>[!MORELIKETHIS]
>
>* [歸因範例1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [歸因範例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [歸因範例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

