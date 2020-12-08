---
unique-page-id: 7515131
description: SFDC同步——刪除銷售線索／聯繫人——行銷文檔——產品文檔
title: SFDC同步——刪除銷售線索／聯繫人
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# SFDC同步：刪除銷售線索／聯繫人 {#sfdc-sync-deleting-a-lead-contact}

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

以下是部分細節：

* Marketo不會因為銷售機會已在Salesforce中刪除而自動刪除人員。 而是將欄位「SFDC已刪除」標誌設定為true。 您可以視需要觸發此欄位以在Marketo中刪除。
* [刪除人員流](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) (Delete Person Flow)操作。 這會刪除MKTO中的人員，但您也可以選擇刪除 `Salesforce` 。

* [從SFDC流動操作中刪除](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) :這會刪除SFDC中的銷售線索，但您也可以選擇刪除Marketo中的人員。
* 如果Salesforce中刪除銷售線索（但Marketo中未刪除人員），接著執行「與Salesforce [](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) flow同步」動作，則會在Salesforce中建立新的銷售線索。

換句話說，它就像魔法一樣！

![--](assets/image2015-5-20-15-3a3-3a27.png)

