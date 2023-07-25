---
unique-page-id: 7515131
description: SFDC同步 — 刪除銷售機會/連絡人 — Marketo檔案 — 產品檔案
title: SFDC同步 — 刪除銷售機會/連絡人
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC同步：刪除銷售機會/連絡人 {#sfdc-sync-deleting-a-lead-contact}

以下是部分詳細資訊：

* Marketo不會因為潛在客戶已在Salesforce中刪除而自動刪除人員。 而是將「SFDC已刪除」欄位標幟設定為true。 您可以視需要觸發此欄位以在Marketo中刪除。
* [刪除人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) 流量動作。 這會刪除MKTO中的人員，但您仍可選擇在中刪除 `Salesforce` 也是。

* [從SFDC刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) 流程動作：這會刪除SFDC中的銷售機會，但您也可以選擇刪除Marketo中的人員。
* 如果銷售機會在Salesforce中刪除(但人員沒有在Marketo中刪除)，然後執行 [與Salesforce同步](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) flow動作，則會在Salesforce中建立新的銷售機會。
