---
unique-page-id: 1147027
description: 將人員同步至SFDC - Marketo檔案 — 產品檔案
title: 將人員同步到SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 1%

---

# 將人員同步到SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>僅在與Salesforce整合時可用。

## 總覽 {#overview}

此流程步驟將插入由Marketo建立的人員，作為銷售機會進入您的Salesforce CRM。

![](assets/sync-person-to-sfdc.png)

## 使用情況 {#usage}

1. 預設情況下，此流步驟將根據Salesforce自動分配規則分配給潛在客戶所有者。

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce要求人員填寫「公司」和「姓氏」欄位。 否則，它將拒絕銷售線索記錄。

1. 您可以將特定的Salesforce用戶或銷售機會隊列設定為銷售機會所有者。

   ![](assets/sync-person-to-sfdc-2.png)

   使用此流程步驟時，系統會立即將人員同步為Salesforce銷售機會，不需要等待定期同步。

   >[!CAUTION]
   >
   >Salesforce不允許將「聯繫人」分配給潛在客戶隊列。 在此情況下，Marketo會在Salesforce中建立重複的「銷售機會」。
