---
unique-page-id: 1147021
description: 變更擁有者 — Marketo檔案 — 產品檔案
title: 變更擁有者
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 變更擁有者 {#change-owner}

如果您的現有人員已指派給擁有者，您可以使用此流程步驟將其重新指派給其他擁有者。

![](assets/image2014-9-22-15-3a1-3a3.png)

**使用情況**

1. 只要選擇您想要變更的擁有者或潛在客戶佇列並開始！

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce不允許將聯絡人指派給潛在客戶佇列。 對於SFDC連絡人記錄：
   >
   >1. Marketo將建立重複的銷售機會 **僅限** 連絡人同步至Salesforce時。 換言之，如果您使用 **[將人員同步至SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流程步驟與 `AssignTo=<a lead queue>`，Marketo會在Salesforce中建立重複的銷售機會，並將其指派給潛在客戶佇列。
   >
   >1. 如果您使用 **變更擁有者** 聯絡人的流程步驟，Marketo會在Salesforce中建立重複的銷售機會。 若要避免此情況，請在「SFDC型別」欄位上使用篩選器，將動作限製為僅限銷售機會。

   >[!NOTE]
   >
   >如果記錄尚未存在於您的Salesforce帳戶中，我們會將其同步化，然後指派給所選使用者。
