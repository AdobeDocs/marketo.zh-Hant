---
unique-page-id: 1147021
description: 變更擁有者 — Marketo檔案 — 產品檔案
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

1. 只需選擇您要更改為的所有者或銷售線索隊列，然後退出！

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce不允許將聯繫人分配給銷售機會隊列。 對於SFDC聯繫人的記錄：
   >
   >1. Marketo將建立重複銷售機會 **僅限** 連絡人同步至Salesforce時。 換句話說，如果您使用 **[將人員同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流步驟 `AssignTo=<a lead queue>`,Marketo會在Salesforce中建立重複的銷售機會，並將其指派至銷售機會佇列。
   >
   >1. 如果您使用 **更改所有者** 在連絡人上執行流程步驟時，Marketo會在Salesforce中建立重複的銷售機會。 要避免此情況，請對「SFDC類型」欄位使用篩選器，該篩選器將操作限制為僅潛在客戶。


   >[!NOTE]
   >
   >如果您的Salesforce帳戶中尚未存在該記錄，我們將將其同步，然後將其分配給選定用戶。
