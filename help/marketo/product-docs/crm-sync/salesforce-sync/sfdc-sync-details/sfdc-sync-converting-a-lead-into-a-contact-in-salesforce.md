---
unique-page-id: 2953465
description: SFDC同步——在Salesforce中將銷售線索轉換為聯繫人-Marketo文檔——產品文檔
title: SFDC同步——在Salesforce中將銷售線索轉換為聯繫人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC同步：在Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}中將銷售線索轉換為聯繫人

請想像Salesforce中的三種不同情形：(不使用Marketo的「轉換人員流程」步驟](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md))[

1. 將Lead轉換為&#x200B;**新聯繫人和新帳戶**
1. 在&#x200B;**現有帳戶**&#x200B;中將Lead轉換為&#x200B;**新聯繫人**

1. 在&#x200B;**現有帳戶**&#x200B;中將Lead轉換為&#x200B;**現有聯繫人**（其工作與[合併](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md)相同）

在這三種情況下，您在Salesforce中都會遇到&#x200B;**1連絡人，沒有潛在客源，在Marketo則會遇到1個連絡人。**

在Marketo，記錄現在將具有SFDC類型=聯繫人。

>[!TIP]
>
>在Salesforce中轉換時，請確定您的[銷售機會自訂欄位已正確映射](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)。 您不想遺失任何資料。

您可以使用下列項目來觸發和篩選：「銷售線索已轉換」和「銷售線索已轉換」。
