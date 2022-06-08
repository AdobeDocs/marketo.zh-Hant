---
unique-page-id: 2953465
description: SFDC同步 — 將Lead轉換為Salesforce中的聯繫人 — Marketo文檔 — 產品文檔
title: SFDC同步 — 在Salesforce中將潛在顧客轉換為聯繫人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC同步：在Salesforce中將Lead轉換為Contact {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想像Salesforce中的三種不同情形：(不使用 [轉換人員流步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) 在Marketo

1. 將Lead轉換為 **新聯繫人和新帳戶**
1. 將Lead轉換為 **新聯繫人** 在 **現有帳戶**

1. 將Lead轉換為 **現有聯繫人** 在 **現有帳戶** (它與 [合併](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

在這三種情況中 **Salesforce有1個聯繫人，沒有線索，Marketo有1個聯繫人，沒有人員。**

在Marketo，記錄現在將具有SFDC類型=聯繫人。

>[!TIP]
>
>在Salesforce中轉換時，請確保 [潛在客戶自定義欄位映射良好](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)。 您不想丟失任何資料。

可以使用：&quot;Lead is Converted&quot;和&quot;Lead is Converted&quot;。
