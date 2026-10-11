---
unique-page-id: 7516241
description: 瞭解如何從Marketo將人員指派給Salesforce銷售機會佇列。 針對銷售機會分配，使用「同步處理人員至SFDC」或「變更擁有者」流程動作。
title: SFDC同步 — 潛在客戶佇列
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/aUrT7qSMy65t3K07O176nt-Bzjm9urgnXKAkZgs1-cs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 6%
---
# SFDC 同步：商機佇列 {#sfdc-sync-lead-queue}

Marketo可讓您將人員新增至[[!DNL Salesforce] 潛在客戶佇列](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm)，以協助進行潛在客戶發佈。 詳情如下。

## 如何在Marketo中將人員指派至佇列？ {#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用下列任一流程動作，將人員指派給[!DNL Salesforce]潛在客戶佇列：

* [將人員同步至 SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [變更所有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>您無法在Marketo中建立或變更佇列。

## 如果人員屬於佇列，要如何儲存潛在客戶擁有者資訊？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果潛在客戶是由[!DNL Salesforce]中的佇列所擁有，這些銷售擁有者欄位會保留空白，直到潛在客戶指派給擁有者為止。

* 銷售擁有者名字
* 銷售負責人姓氏
* 銷售擁有者職稱
* 銷售負責人電話號碼
* 銷售負責人電子郵件地址
