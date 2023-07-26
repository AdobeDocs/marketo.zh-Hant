---
unique-page-id: 7514149
description: 歸因範例3 - Marketo檔案 — 產品檔案
title: 歸因範例3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# 歸因範例3 {#attribution-example}

請閱讀下列情境，並嘗試決定網格中應該包含的數字。

* 4月11日 | Steve下載（內容） — 成功
* 4月22日 |機會是以$3,000建立（Steve和Jason都有角色）
* 4月25日 | Jason出席（網路研討會） — 成功
* 4月30日 |商機已結束 — 成功

| 歸因量度 | (內容) | （網路研討會） |
|---|---|---|
| (MT)建立的商機 | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT)管道已建立 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT)韓圜 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT)贏得的收入 | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**顯示答案**

>[!NOTE]
>
>**說明**
>
>記住歸因規則#3。 Jason在建立商機之後就取得計畫成功。 因此，網路研討會無法取得機會建立的評分。 僅限贏取商機的銷退折讓。
>
>因此，（內容）會將100%的點數歸於商機建立與管道，但只將50%的點數歸於贏得的商機。

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
>* [歸因範例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
