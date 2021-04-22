---
unique-page-id: 1147031
description: 從SFDC刪除人員-Marketo文檔——產品文檔
title: 從SFDC刪除人員
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 從SFDC {#delete-person-from-sfdc}刪除人員

如果您需要從Salesforce中刪除一組特定的銷售線索，但將其保留為Marketo地區的人員，則可以使用「從SFDC流程中刪除人員」活動。

>[!NOTE]
>
>僅在與Salesforce整合時提供。

1. 在「資料庫」中，按一下您要從Salesforce移除的人員。 然後按一下「**人員動作**」，並選取「**Salesforce**」。

   ![](assets/person-actions-salesforce.png)

1. 選擇&#x200B;**從SFDC**&#x200B;刪除人員。

   ![](assets/delete-person-from-sfdc.png)

1. 請確定「在Marketo刪除」設定為「**false**」，然後按一下「立即執行」。********

   ![](assets/run-action-delete-lead-from-sfdc.png)

   流程步驟執行後，您的人員將不再是Salesforce的領導者，而將留在Marketo。

   >[!CAUTION]
   >
   >如果您將Marketo的&#x200B;**Delete設為** true **，並刪除Marketo的人員和Salesforce的銷售線索，這些線索將永遠消失。**&#x200B;這是無法復原的。
