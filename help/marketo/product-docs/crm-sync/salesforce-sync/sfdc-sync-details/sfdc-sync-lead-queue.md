---
unique-page-id: 7516241
description: SFDC同步 — 潛在客戶隊列 — Marketo文檔 — 產品文檔
title: SFDC同步 — 潛在客戶隊列
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# SFDC同步：潛在客戶隊列 {#sfdc-sync-lead-queue}

Marketo允許你將人添加到 [Salesforce潛在顧客隊列](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) 幫助銷售線索分配。 詳情請看。

## 如何將人員分配到Marketo的隊列？ {#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用以下任一流動活動將人員分配給Salesforce潛在客戶隊列：

* [將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>無法在Marketo建立或更改隊列。

## 如果人員屬於隊列，則如何儲存潛在顧客所有者資訊？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果Salesforce中的隊列擁有潛在顧客，則這些銷售責任人欄位將保持為空，直到將潛在顧客分配給責任人。

* 銷售所有者名
* 銷售所有者姓
* 銷售所有者標題
* 銷售所有者電話號碼
* 銷售所有者電子郵件地址
