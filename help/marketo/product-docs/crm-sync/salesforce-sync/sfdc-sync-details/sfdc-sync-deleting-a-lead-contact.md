---
unique-page-id: 7515131
description: SFDC同步 — 刪除潛在客戶/聯繫人 — Marketo文檔 — 產品文檔
title: SFDC同步 — 刪除潛在顧客/聯繫人
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC同步：刪除潛在顧客/聯繫人 {#sfdc-sync-deleting-a-lead-contact}

下面是一些細節：

* Marketo不會僅僅因為Salesforce中刪除了線索就自動刪除人員。 而是將欄位「SFDC已刪除」標誌設定為true。 如果需要，可觸發此欄位以在Marketo刪除。
* [刪除人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) 流操作。 這將刪除MKTO中的人員，但您可以選擇在中刪除 `Salesforce` 也。

* [從SFDC刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) 流操作：這將刪除SFDC中的潛在顧客，但您也可以選擇刪除Marketo的人。
* 如果在Salesforce中刪除了潛在顧客(但在Marketo中未刪除人員)，然後通過 [與Salesforce同步](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 流程操作，然後在Salesforce中建立新的潛在客戶。
