---
unique-page-id: 7514151
description: 歸因範例4 - Marketo檔案 — 產品檔案
title: 歸因範例4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 歸因範例4 {#attribution-example}

請閱讀下列情境，並嘗試決定網格中應該包含的數字。

* 4月11日 |米歇爾下載電子書（內容） — 成功
* 4月15日 | John attends （網路研討會） — 成功
* 4月22日 | （商機1）已建立為$3,000
* 4月24日 | （商機2）已建立為$5,000
* 4月25日 |約翰和米歇爾關聯至 **兩者** Optys
* 4月29日 | [光碟機1] 為已結束 — 已結束

| 計畫名稱 | (內容) | （網路研討會） |
|---|---|---|
|   | （光碟機1） | （光碟機2） | （光碟機1） | （光碟機2） |
| (MT)建立的商機 | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)管道已建立 | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT)韓圜 | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT)贏得的收入 | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**顯示答案**

>[!NOTE]
>
>**說明**
>
>當您有多個機會和多個人員取得方案成功時，您必須在人員和方案之間分割評分。 但是，請注意，機會1和2的評分不會合併。 每個都是不同的評分評估。
>
>涉及許多人時，Marketo會自動計算可給予評分之機會的分數。

>[!NOTE]
>
>**歸因規則**
>
>1. 評分會平均分割
>1. 您獲得的評分不能超過您獲得的評分
>1. 您無法為過去發生的事件給予評價

嘗試所有範例，您就會成為歸因專家！

>[!MORELIKETHIS]
>
>* [歸因範例1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [歸因範例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [歸因範例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
