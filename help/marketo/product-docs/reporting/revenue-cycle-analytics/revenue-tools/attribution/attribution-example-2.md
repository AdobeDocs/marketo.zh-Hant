---
unique-page-id: 7514146
description: 歸因範例2 - Marketo檔案 — 產品檔案
title: 歸因範例2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 歸因範例2 {#attribution-example}

請閱讀下列情境，並嘗試決定網格中應該包含的數字。

* 4月11日 | 帳單取得者（商展）
* 4月15日 | 瓊已獲得（網路研討會）
* 4月22日 | （商機1）已建立為$6,000
* 4月24日 | 以$10,000建立的（商機2）
* 4月25日 | Bill和Joan與&#x200B;**BOTH**&#x200B;選項的角色相關聯
* 4月29日 | （商機1）已結束獲勝

| 計畫名稱 | （商展） | （網路研討會） |
|---|---|---|
| (FT)已建立商機 | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT)管道已建立 | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT)韓冠廷 | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT)贏得的收入 | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**顯示答案**

>[!NOTE]
>
>**說明**
>
>因為Bill和Joan都與&#x200B;**BOTH**&#x200B;商機的角色相關聯，所以系統（根據規則）會平均分割他們之間的評分。
>
>為每個方案建立的管道($8,000)是可用信用額度總數($16,000)的一半。

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
>* [歸因範例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [歸因範例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
