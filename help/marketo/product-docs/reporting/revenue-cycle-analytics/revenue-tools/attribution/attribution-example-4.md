---
unique-page-id: 7514151
description: 歸因範例4 - Marketo檔案 — 產品檔案
title: 歸因範例4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 歸因範例4 {#attribution-example}

請閱讀以下案例，並嘗試確定網格中應包含的數字。

* 4月11日 | Michelle下載電子書（內容） — 成功
* 4月15日 | John到場（網路研討會） — 成功
* 4月22日 |（機會1）為3,000美元建立
* 4月24日 |（機會2）為5,000美元建立
* 4月25日 |約翰和米歇爾與 **both** 奧普蒂
* 4月29日 | [第1] 為閉原

| 方案名稱 | (內容) | （網路研討會） |
|---|---|---|
|  | （第1項） | （第2項） | （第1項） | （第2項） |
| (MT)已建立Opty | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)管道已建立 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)奧蒂元 | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)收入成本 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**顯示答案**

>[!NOTE]
>
>**說明**
>
>當您有多個機會和多個人員且計畫成功時，您必須將人員和計畫之間的評分分開。 但是，請注意，機會1和2的評分不會合併。 每個都是一個獨特的信用評估。
>
>當有許多人參與時，Marketo會自動電腦會中可給予評分的部分。

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
>* [歸因範例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)

