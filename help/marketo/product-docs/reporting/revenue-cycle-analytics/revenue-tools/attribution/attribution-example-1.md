---
unique-page-id: 7514126
description: 歸因範例1 - Marketo檔案 — 產品檔案
title: 歸因範例1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 歸因範例1 {#attribution-example}

請閱讀下列情境，並嘗試決定網格中應該包含的數字。

* 4月11日 |Fred被（商展）收購
* 4月15日 | Margo attends （網路研討會） — 成功
* 4月22日 | Fred已與此機會建立關聯（角色）
* 4月22日 |機會建立費用為$3,000

| 計畫名稱 | （商展） | （網路研討會） |
|---|---|---|
| (FT)已建立商機 | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT)管道已建立 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT)韓冠廷 | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT)贏得的收入 | `<pre>0</pre>` | `<pre>0</pre>` |

**顯示答案**

>[!NOTE]
>
>**說明**
>
>首先，瞭解部分型別為COUNTS，其他型別為CURRENCY。 建立的機會是計數，一個整數。 Pipeline是貨幣。 在Marketo中，貨幣將符合您的管理員地區設定。
>
>商展獲得所有評分的原因是Margo與商機中的角色沒有關聯。 沒有角色，沒有功勞。

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
>* [歸因範例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [歸因範例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [歸因範例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
