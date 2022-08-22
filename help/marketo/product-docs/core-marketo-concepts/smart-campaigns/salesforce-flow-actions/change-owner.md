---
unique-page-id: 1147021
description: 更改所有者 — Marketo文檔 — 產品文檔
title: 更改所有者
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
source-git-commit: 44c134811242b4136a3137cdd60e60edeb838c8c
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 更改所有者 {#change-owner}

如果現有人員已分配給某個所有者，則可以使用此流步驟將他們重新分配給另一個所有者。

![](assets/image2014-9-22-15-3a1-3a3.png)

**使用情況**

1. 您只需選擇要更改為的所有者或潛在顧客隊列，然後繼續！

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce不允許將聯繫人分配給潛在顧客隊列。 對於SFDC聯繫人的記錄：
   >
   >1. Marketo將建立重複的線索 **僅** 當聯繫人同步到Salesforce時。 換句話說，如果你用 **[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流步 `AssignTo=<a lead queue>`,Marketo將在Salesforce中建立重複的潛在顧客並將其分配給潛在顧客隊列。
   >
   >1. 如果使用 **更改所有者** 在聯繫人上執行流步驟，Marketo在Salesforce中建立重複的潛在客戶。 為避免這種情況，請在「SFDC類型」欄位上使用一個篩選器，該篩選器將操作限制為僅限於潛在顧客。


   >[!NOTE]
   >
   >如果Salesforce帳戶中尚未存在該記錄，我們將同步該記錄，然後將其分配給選定用戶。
