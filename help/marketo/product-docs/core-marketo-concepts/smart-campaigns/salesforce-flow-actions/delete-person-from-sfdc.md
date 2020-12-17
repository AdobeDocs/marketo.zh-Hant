---
unique-page-id: 1147031
description: 從SFDC刪除人員——行銷人員文檔——產品文檔
title: 從SFDC刪除人員
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---


# 從SFDC {#delete-person-from-sfdc}刪除人員

如果您需要從Salesforce中刪除一組特定的銷售線索，但將它們留作Marketo中的人員，則可以使用「從SFDC流程中刪除人員」操作。

>[!NOTE]
>
>僅在與Salesforce整合時提供。

1. 在「資料庫」中，按一下您要從Salesforce移除的人員。 然後按一下「**人員動作**」，並選取「**Salesforce**」。

   ![](assets/person-actions-salesforce.png)

1. 選擇&#x200B;**從SFDC**&#x200B;刪除人員。

   ![](assets/delete-person-from-sfdc.png)

1. 請確定「在Marketo中刪除」設定為「**false**」，然後按一下「立即執行」。********

   ![](assets/run-action-delete-lead-from-sfdc.png)

   流程步驟執行後，您的人員將不再是Salesforce中的銷售線索，而將繼續留在Marketo中。

   >[!CAUTION]
   >
   >如果您在Marketo中將&#x200B;**Delete**&#x200B;設為&#x200B;**true**，並將人員從Marketo和Salesforce中刪除，則他們將永遠消失。 這是無法復原的。

