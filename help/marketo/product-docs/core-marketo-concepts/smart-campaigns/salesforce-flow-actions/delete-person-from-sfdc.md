---
unique-page-id: 1147031
description: 瞭解如何透過流程步驟從Salesforce刪除人員。 當潛在客戶或連絡人進入流程時，從SFDC中將其移除。
title: 從 SFDC 中刪除人員
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/f-Zvc4glfCtAagE314vrZjiWIcD3vaGIKmKGeZO18v0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 133
ht-degree: 6%

---

# 從 SFDC 中刪除人員 {#delete-person-from-sfdc}

如果您需要從Salesforce中移除一組特定的銷售機會，但保留為Marketo Engage中的人員，則可以使用從SFDC流程刪除人員動作。

>[!NOTE]
>
>僅在與[!DNL Salesforce]整合時可用。

1. 在資料庫中，按一下您要從Salesforce移除的人員。 然後按一下&#x200B;**[!UICONTROL Person Actions]**&#x200B;並選取&#x200B;**[!DNL Salesforce]**。

   ![](assets/delete-person-from-sfdc-1.png)

1. 選取「**[!UICONTROL Delete Person from SFDC]**」。

   ![](assets/delete-person-from-sfdc-2.png)

1. 確定&#x200B;**[!UICONTROL Delete in Marketo]**&#x200B;設定為&#x200B;**[!UICONTROL false]**，然後按一下&#x200B;**[!UICONTROL Run Now]**。

   ![](assets/delete-person-from-sfdc-3.png)

   流程步驟執行後，您的人員將不再是[!DNL Salesforce]中的銷售機會，但將保留在Marketo中。

   >[!CAUTION]
   >
   >如果您將&#x200B;**[!UICONTROL Delete in Marketo]**&#x200B;設為&#x200B;**[!UICONTROL true]**&#x200B;並從Marketo中刪除人員和Salesforce的銷售機會，則為永久性刪除。 此動作無法還原。
