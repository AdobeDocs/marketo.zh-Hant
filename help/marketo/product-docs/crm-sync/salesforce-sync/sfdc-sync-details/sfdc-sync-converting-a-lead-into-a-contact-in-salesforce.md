---
unique-page-id: 2953465
description: SFDC Sync — 在Salesforce中將銷售機會轉換為聯絡人 — Marketo檔案 — 產品檔案
title: SFDC Sync — 在Salesforce中將銷售機會轉換為聯絡人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC同步：在Salesforce中將銷售機會轉換為聯絡人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想像一下Salesforce中的三種不同情況：(不使用 [轉換人員流程步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) (在Marketo)

1. 將銷售機會轉換為 **新連絡人和新帳戶**
1. 將銷售機會轉換為 **新連絡人** 在 **現有帳戶**

1. 將銷售機會轉換為 **現有連絡人** 在 **現有帳戶** (此功能的運作方式與 [合併](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

在所有三個案例中，您最終都會獲得 **Salesforce中有1個聯絡人且沒有銷售機會，Marketo中有1個聯絡人且沒有人員。**

在Marketo中，記錄現在會有SFDC Type = Contact。

>[!TIP]
>
>在Salesforce中轉換時，請確定 [潛在客戶自訂欄位對應良好](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). 您不想遺失任何資料。

您可使用：「已轉換潛在客戶」和「已轉換潛在客戶」來觸發及篩選。
