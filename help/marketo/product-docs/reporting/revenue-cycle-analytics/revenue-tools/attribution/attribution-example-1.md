---
unique-page-id: 7514126
description: 歸因範例1 - Marketo檔案 — 產品檔案
title: 歸因範例1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 歸因範例1 {#attribution-example}

請閱讀以下案例，並嘗試確定網格中應包含的數字。

* 4月11日 | Fred由收購（展會）
* 4月15日 | Margo參加（網路研討會） — 成功
* 4月22日 | Fred與銷售機會相關聯（角色）
* 4月22日 |為3,000美元建立了銷售機會

| 方案名稱 | （展會） | （網路研討會） |
|---|---|---|
| (FT)已建立Opty | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT)管道已建立 | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT)奧蒂元 | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT)收入韓元 | `<pre>0</pre>` | `<pre>0</pre>` |

**顯示答案**

>[!NOTE]
>
>**說明**
>
>首先，請了解某些類型為COUNTS，而其他類型為CURRENCY。 Opty Created是計數，是整數。 管道是一種貨幣。 在Marketo中，貨幣會符合您的管理員地區設定。
>
>Tradeshow獲得所有評分的原因是Margo未與機會中的角色關聯。 沒有角色，沒有信用。

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
>* [歸因範例2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [歸因範例3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [歸因範例4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

