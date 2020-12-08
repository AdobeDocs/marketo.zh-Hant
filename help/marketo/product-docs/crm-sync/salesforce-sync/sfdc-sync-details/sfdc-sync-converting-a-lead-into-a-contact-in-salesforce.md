---
unique-page-id: 2953465
description: SFDC同步——在Salesforce中將銷售線索轉換為聯繫人——行銷人員文檔——產品文檔
title: SFDC同步——在Salesforce中將銷售線索轉換為聯繫人
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# SFDC同步：在Salesforce中將銷售線索轉換為聯繫人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

請想像Salesforce中的三種不同情形：(不使用Marketo中 [的「轉換人員流程](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) 」步驟)

1. 將Lead轉換為新的 **連絡人和新帳戶**
1. 將Lead轉換為現有 **帳戶中的** 新 **聯繫人**

1. 將Lead轉換為現 **有帳戶中****的現有聯繫人** (這與合 [並相同](sfdc-sync-merging-a-lead-contact-person.md))

在這三種情況下，您在Salesforce中都只有 **1個連絡人，沒有潛在客戶，在Marketo中則有1個連絡人，沒有人員。**

在Marketo中，記錄現在將具有SFDC類型=聯繫人。

>[!TIP]
>
>在Salesforce中轉換時，請確定您的銷 [售機會自訂欄位已正確對應](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)。 您不想遺失任何資料。

您可以使用下列項目來觸發和篩選：「銷售線索已轉換」和「銷售線索已轉換」。