---
unique-page-id: 1147021
description: 變更擁有者 — Marketo檔案 — 產品檔案
title: 變更所有者
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 2%

---

# 變更所有者 {#change-owner}

如果您的現有人員已指派給擁有者，您可以使用此流程步驟將其重新指派給其他擁有者。

![](assets/change-owner-1.png)

1. 只要選擇您想要變更的擁有者或潛在客戶佇列並開始！

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >[!DNL Salesforce]不允許將連絡人指派給潛在客戶佇列。 若記錄為SFDC聯絡人：
   >
   >* 當連絡人同步至Salesforce時，Marketo僅會建立重複的銷售機會&#x200B;**1&rbrace;。**&#x200B;換言之，如果您搭配&#x200B;**[使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**&#x200B;將人員同步至SFDC`AssignTo=<a lead queue>`流程步驟，Marketo將在Salesforce中建立重複的銷售機會，並將其指派給銷售機會佇列。
   >
   >* 如果您在聯絡人上使用&#x200B;**[!UICONTROL Change Owner]**&#x200B;流程步驟，Marketo會在Salesforce中建立重複的銷售機會。 若要避免此問題，請在「SFDC型別」欄位上使用篩選器，將動作限製為僅限銷售機會。

   >[!NOTE]
   >
   >如果記錄尚未存在於您的[!DNL Salesforce]帳戶中，我們會將其同步處理，然後將其指派給選取的使用者。
