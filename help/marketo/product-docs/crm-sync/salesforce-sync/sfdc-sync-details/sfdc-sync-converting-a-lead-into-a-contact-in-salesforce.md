---
unique-page-id: 2953465
description: SFDC同步——在Salesforce中將銷售線索轉換為聯繫人——行銷人員文檔——產品文檔
title: SFDC同步——在Salesforce中將銷售線索轉換為聯繫人
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# SFDC同步：在Salesforce中將銷售線索轉換為聯繫人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

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