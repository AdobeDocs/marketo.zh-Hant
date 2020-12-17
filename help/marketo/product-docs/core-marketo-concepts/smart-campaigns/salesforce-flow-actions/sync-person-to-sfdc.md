---
unique-page-id: 1147027
description: 將人員同步至SFDC —— 行銷人員文檔——產品文檔
title: 將人員同步到SFDC
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# 將人員同步到SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>僅在與Salesforce整合時提供。

## 概述{#overview}

此流程步驟會將行銷人員建立的人員插入您的Salesforce CRM。

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

