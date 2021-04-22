---
unique-page-id: 7516241
description: SFDC同步——銷售線索隊列-Marketo文檔——產品文檔
title: SFDC同步——銷售線索隊列
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# SFDC同步：Lead Queue {#sfdc-sync-lead-queue}

Marketo允許您將人員添加到[Salesforce銷售線索隊列](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm)以幫助銷售線索分配。 以下是詳細資訊。

## 如何指派人員到Marketo的佇列？{#how-to-assign-a-person-to-a-queue-in-marketo}

您可以使用下列其中一個流程動作，將人員指派給Salesforce銷售線索佇列：

* [將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [變更擁有者](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>您不能在Marketo建立或更改隊列。

## 如果銷售線索擁有者資訊屬於隊列，該資訊如何儲存？{#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

如果Salesforce中的佇列擁有銷售線索，這些銷售擁有者欄位會保持空白，直到將銷售線索指派給擁有者為止。

* 銷售擁有者名字
* 銷售擁有者姓氏
* 銷售擁有者標題
* 銷售人員電話號碼
* 銷售擁有者電子郵件地址
