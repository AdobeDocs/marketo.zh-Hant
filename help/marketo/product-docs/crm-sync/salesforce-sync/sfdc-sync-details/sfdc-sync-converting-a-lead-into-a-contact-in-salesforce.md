---
unique-page-id: 2953465
description: SFDC同步 — 在Salesforce中將銷售機會轉換為聯繫人 — Marketo文檔 — 產品文檔
title: SFDC同步 — 在Salesforce中將銷售機會轉換為聯繫人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC同步：在Salesforce中將銷售機會轉換為聯繫人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想像一下Salesforce中的三種情況：(未使用 [轉換人員流程步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) 在Marketo)

1. 將銷售機會轉換為 **新聯繫人和新帳戶**
1. 將銷售機會轉換為 **新聯繫人** 在 **現有帳戶**

1. 將銷售機會轉換為 **現有聯繫人** 在 **現有帳戶** (此功能與 [合併](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

在這三種情況下 **Salesforce中有1個連絡人，沒有線索，Marketo中有1個連絡人，沒有人。**

在Marketo中，記錄現在會有SFDC類型=連絡。

>[!TIP]
>
>在Salesforce中進行轉換時，請確定 [潛在客戶自訂欄位已完全對應](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). 您不想遺失任何資料。

您可以使用：&quot;銷售機會已轉換&quot;和&quot;銷售機會已轉換&quot;。&quot;
