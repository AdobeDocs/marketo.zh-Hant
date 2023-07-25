---
unique-page-id: 1147027
description: 將人員同步至SFDC - Marketo檔案 — 產品檔案
title: 將人員同步至SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 1%

---

# 將人員同步至SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>僅在與Salesforce整合時可用。

## 概觀 {#overview}

此流程步驟會將Marketo建立的人作為銷售機會插入您的Salesforce CRM。

![](assets/sync-person-to-sfdc.png)

## 使用情況 {#usage}

1. 依預設，此流程步驟會根據Salesforce自動指定規則指定給潛在客戶擁有者。

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce要求人員填寫公司和姓氏欄位。 否則，會拒絕潛在客戶記錄。

1. 您可以將特定的Salesforce使用者或銷售機會佇列設定為銷售機會擁有者。

   ![](assets/sync-person-to-sfdc-2.png)

   使用此流程步驟時，人員會立即同步為Salesforce銷售機會，不需要等候一般同步。

   >[!CAUTION]
   >
   >Salesforce不允許將「連絡人」指派給潛在客戶佇列。 在此情況下，Marketo會在Salesforce中建立重複的「銷售機會」。
