---
unique-page-id: 7514151
description: 歸因範例4 —— 行銷人員檔案——產品檔案
title: 歸因範例4
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# 歸因範例4 {#attribution-example}

請閱讀以下案例，並嘗試判斷應該在格線中的數字。

* 4月11日 | Michelle下載電子書（內容）-成功
* 4月15日 | John參加（網路研討會）-成功
* 4月22日 |(Opportunity 1)以$3,000建立
* 4月24日 |(Opportunity 2)以$5,000建立
* 4月25日 | John和Michelle與&#x200B;**both** Optys關聯
* 4月29日 | [Opty 1]是Closed-Won

| 方案名稱 | （內容） | （網路研討會） |
|---|---|---|
|  | （第1項） | （第2項） | （第1項） | （第2項） |
| (MT)已建立選項 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)已建立管線 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)贏取收入 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**顯示答案**

>[!NOTE]
>
>**說明**
>
>當您擁有多個機會和多個成功參與計畫的人員時，您必須將人員和計劃分開。 但是，請注意，機會1和機會2的評分不會合併。 每個評估都是一個明確的信用評估。
>
>當有許多人參與時，Marketo會自動電腦會的分數，以給予評價。

>[!NOTE]
>
>**歸因規則**
>
>1. 平均分配評分
>1. 你不能比你掙的錢多
>1. 你不能因為過去發生的事而自責


請試用所有範例，您就是歸因專家！

>[!MORELIKETHIS]
>
>* [歸因範例1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [歸因範例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [歸因範例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)

