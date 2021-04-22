---
unique-page-id: 7515131
description: SFDC同步——刪除銷售線索／聯繫人-Marketo文檔——產品文檔
title: SFDC同步——刪除銷售線索／聯繫人
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC同步：刪除銷售線索／聯繫人{#sfdc-sync-deleting-a-lead-contact}

以下是部分細節：

* Marketo不會因為銷售機會在Salesforce中刪除而自動刪除人員。 而是將欄位「SFDC已刪除」標誌設定為true。 您可以視需要觸發此欄位以在Marketo刪除。
* [刪除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) 人員流動操作。這會刪除MKTO中的人員，但您也可以選擇在`Salesforce`中刪除。

* [從](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow操作刪除：這會刪除SFDC中的銷售線索，但您也可以選擇刪除Marketo的人員。
* 如果銷售線索在Salesforce中刪除(但在Marketo不刪除)，然後透過[與Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流動動作同步，則會在Salesforce中建立新的銷售線索。
