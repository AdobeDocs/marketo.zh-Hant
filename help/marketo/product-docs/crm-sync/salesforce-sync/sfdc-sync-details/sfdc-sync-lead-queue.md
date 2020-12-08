---
unique-page-id: 7516241
description: SFDC同步——銷售線索隊列——行銷文檔——產品文檔
title: SFDC同步——銷售線索隊列
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# SFDC同步：銷售線索隊列 {#sfdc-sync-lead-queue}

Marketo可讓您將人員新增至 [Salesforce銷售線索佇列](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) ，以協助銷售線索分配。 以下是詳細資訊。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## 如何指派人員至Marketo中的佇列？ {#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用下列其中一個流程動作，將人員指派給Salesforce銷售線索佇列：

* [將人員同步到SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [變更擁有者](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>您無法在Marketo中建立或變更佇列。

## 如果銷售線索擁有者資訊屬於隊列，該資訊如何儲存？ {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果Salesforce中的佇列擁有銷售線索，這些銷售擁有者欄位會保持空白，直到銷售線索指派給擁有者為止。

* 銷售擁有者名字
* 銷售擁有者姓氏
* 銷售擁有者標題
* 銷售人員電話號碼
* 銷售擁有者電子郵件地址

