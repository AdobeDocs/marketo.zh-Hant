---
unique-page-id: 7515131
description: SFDC同步 — 刪除銷售機會/連絡人 — Marketo檔案 — 產品檔案
title: SFDC同步 — 刪除銷售機會/連絡人
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# SFDC同步：刪除銷售機會/連絡人 {#sfdc-sync-deleting-a-lead-contact}

以下是部分詳細資訊：

* Marketo不會因為潛在客戶已在[!DNL Salesforce]中刪除而自動刪除人員。 而「SFDC已刪除」欄位標幟已設為true。 您可以視需要觸發此欄位以在Marketo中刪除。
* [刪除人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md)流程動作。 這會刪除MKTO中的人員，但您也可以選擇刪除`Salesforce`中的人員。

* [從SFDC刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md)流程動作：這將刪除SFDC中的銷售機會，但您也可以選擇刪除Marketo中的人員。
* 如果在[!DNL Salesforce]中刪除銷售機會(但未在Marketo中刪除人員)，然後執行[與 [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流程同步動作，則會在[!DNL Salesforce]中建立新的銷售機會。
