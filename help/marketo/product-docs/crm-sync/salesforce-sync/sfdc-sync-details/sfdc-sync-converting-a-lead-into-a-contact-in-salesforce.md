---
unique-page-id: 2953465
description: SFDC Sync — 在Salesforce中將銷售機會轉換為聯絡人 — Marketo檔案 — 產品檔案
title: SFDC Sync — 在Salesforce中將銷售機會轉換為聯絡人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# SFDC同步：在Salesforce中將銷售機會轉換為聯絡人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想像一下Salesforce中的三種不同情境： (不使用Marketo Engage中的[轉換人員流程步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"})

1. 正在將Lead轉換為&#x200B;**新連絡人和新帳戶**
1. 正在將Lead轉換為&#x200B;**現有帳戶**&#x200B;中的&#x200B;**新連絡人**

1. 正在將Lead轉換為&#x200B;**現有帳戶**&#x200B;中的&#x200B;**現有連絡人** （此運作方式與[合併](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"}相同）

在所有三個案例中，您最終在Salesforce中有&#x200B;**1個連絡人，沒有銷售機會，在Marketo中有1個連絡人，沒有人員。**

在Marketo中，記錄現在會有SFDC Type = Contact。

>[!TIP]
>
>在Salesforce中轉換時，請確定您的[潛在客戶自訂欄位已對應妥當](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}。 您不想遺失任何資料。

您可使用：「已轉換潛在客戶」和「已轉換潛在客戶」來觸發及篩選。
