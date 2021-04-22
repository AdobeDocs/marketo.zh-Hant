---
unique-page-id: 1147021
description: 變更擁有者-Marketo檔案——產品檔案
title: 變更擁有者
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# 更改所有者{#change-owner}

如果現有人員已分配給所有者，則可以使用此流程步驟將他們重新分配給其他所有者。

![](assets/image2014-9-22-15-3a1-3a3.png)

**使用狀況**

1. 只要挑選您要變更的擁有者或潛在客戶佇列，就可以了！

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce不允許將聯繫人指派給銷售線索隊列。 對於SFDC聯繫人記錄：
   >
   >1. 當連絡人同步至Salesforce時，Marketo將只建立重複的潛在客戶&#x200B;****。 換言之，如果您使用&#x200B;**[將人員同步至SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**&#x200B;流程步驟與`AssignTo=<a lead queue>`,Marketo將在Salesforce中建立重複的銷售線索，並將其指派至銷售線索佇列。
      >
      >
   1. 如果您嘗試在連絡人上使用&#x200B;**變更擁有者**&#x200B;流程步驟，Salesforce中將不會建立任何重複項目。


   >[!NOTE]
   >
   >如果您的Salesforce帳戶中尚未存在記錄，我們會將記錄同步，然後將它指派給選取的使用者。
