---
unique-page-id: 1147031
description: 從SFDC刪除人員——行銷人員文檔——產品文檔
title: 從SFDC刪除人員
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# 從SFDC刪除人員 {#delete-person-from-sfdc}

如果您需要從Salesforce中刪除一組特定的銷售線索，但將它們留作Marketo中的人員，則可以使用「從SFDC流程中刪除人員」操作。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>僅在與Salesforce整合時提供。

1. 在「資料庫」中，按一下您要從Salesforce移除的人員。 然後按一 **下「人員動作** 」，並選 **取「Salesforce**」。

   ![](assets/person-actions-salesforce.png)

1. 選擇 **從SFDC刪除人員**。

   ![](assets/delete-person-from-sfdc.png)

1. 請確定「在Marketo **中刪除** 」設 **定為false**，然後按一下「 **立即執行**」。

   ![](assets/run-action-delete-lead-from-sfdc.png)

   流程步驟執行後，您的人員將不再是Salesforce中的銷售線索，而將繼續留在Marketo中。

   >[!CAUTION]
   >
   >如果您在Marketo **中將Delete** （刪除）設 **為True** ，並從Marketo刪除人員，以及從Salesforce刪除銷售機會，則他們將永遠消失。 這是無法復原的。

