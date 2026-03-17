---
unique-page-id: 1147027
description: 瞭解如何使用流程步驟將人員同步至Salesforce。 潛在客戶或聯絡資料進入流量時，將資料推送至SFDC。
title: 將人員同步至 SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 5%

---

# 將人員同步至 SFDC {#sync-person-to-sfdc}

此流程步驟會將Marketo建立的人員當作銷售機會插入您的Salesforce CRM。

>[!NOTE]
>
>僅在與[!DNL Salesforce]整合時可用。

1. 依預設，此流程步驟會根據Salesforce自動指派規則指派給潛在客戶擁有者。

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce]要求人員填寫公司和姓氏欄位。 否則，它會拒絕潛在客戶記錄。

1. 您可以將特定的[!DNL Salesforce]使用者或潛在客戶佇列設定為潛在客戶擁有者。

   ![](assets/sync-person-to-sfdc-2.png)

   使用此流程步驟時，人員會立即同步為[!DNL Salesforce]銷售機會，不需要等候定期同步。

   >[!CAUTION]
   >
   >[!DNL Salesforce]不允許將「連絡人」指派給潛在客戶佇列。 在此情況下，Marketo將在[!DNL Salesforce]中建立重複的「銷售機會」。
