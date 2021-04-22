---
unique-page-id: 1147027
description: 將人員同步到SFDC -Marketo文檔——產品文檔
title: 將人員同步到SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---

# 將人員同步到SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>僅在與Salesforce整合時提供。

## 概述{#overview}

此流程步驟會將由Marketo建立的人員插入您的Salesforce CRM中，作為客源。

![](assets/sync-person-to-sfdc.png)

## 用法{#usage}

1. 依預設，此流程步驟會根據Salesforce自動指派規則指派給銷售線索擁有者。

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce要求人員填寫「公司」和「姓氏」欄位。 否則，它將拒絕銷售線索記錄。

1. 您可以將特定Salesforce使用者或銷售線索佇列設為銷售線索擁有者。

   ![](assets/sync-person-to-sfdc-2.png)

   使用此流程步驟時，人員會立即同步為Salesforce銷售線索，而不需等候定期同步。

   >[!CAUTION]
   >
   >Salesforce不允許將「連絡人」指派給銷售線索佇列。 在這種情況下，Marketo會在Salesforce中建立重複的「銷售機會」。
