---
unique-page-id: 7516241
description: SFDC同步 — 銷售機會隊列 — Marketo文檔 — 產品文檔
title: SFDC同步 — 銷售機會隊列
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# SFDC同步：銷售機會隊列 {#sfdc-sync-lead-queue}

Marketo可讓您將人員新增至 [Salesforce銷售機會隊列](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) 協助銷售機會分發。 詳情如下。

## 如何在Marketo中將人員指派至佇列？ {#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用以下任一流程操作將人員分配給Salesforce銷售線索隊列：

* [將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [更改所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>您無法在Marketo中建立或變更佇列。

## 如果人員屬於隊列，如何儲存銷售機會所有者資訊？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果銷售線索由Salesforce中的隊列擁有，則這些銷售責任人欄位將保持空白，直到銷售線索被分配給責任人。

* 銷售負責人名字
* 銷售責任人姓氏
* 銷售所有者標題
* 銷售負責人電話號碼
* 銷售所有者電子郵件地址
