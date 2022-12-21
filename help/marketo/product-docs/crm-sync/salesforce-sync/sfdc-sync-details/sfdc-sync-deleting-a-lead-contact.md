---
unique-page-id: 7515131
description: SFDC同步 — 刪除銷售機會/聯繫人 — Marketo文檔 — 產品文檔
title: SFDC同步 — 刪除銷售機會/聯繫人
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC同步：刪除銷售機會/連絡人 {#sfdc-sync-deleting-a-lead-contact}

以下是部分細節：

* Marketo不會因為銷售機會在Salesforce中刪除而自動刪除人員。 而將欄位「SFDC已刪除」標幟設為true。 您可以視需要觸發此欄位以在Marketo中刪除。
* [刪除人員](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) 流量動作。 這會刪除MKTO中的人員，但您可以在 `Salesforce` 也是。

* [從SFDC中刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) 流量動作：這會刪除SFDC中的銷售機會，但您也可以選擇刪除Marketo中的人員。
* 如果銷售機會在Salesforce中刪除(但Marketo中未刪除人員)，然後在 [與Salesforce同步](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 流程動作，則會在Salesforce中建立新銷售機會。
