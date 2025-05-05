---
unique-page-id: 1147031
description: 從SFDC刪除人員 — Marketo檔案 — 產品檔案
title: 從SFDC刪除人員
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 從SFDC刪除人員 {#delete-person-from-sfdc}

如果您需要從Salesforce移除特定銷售機會集，但保留為Marketo Engage中的人員，則可使用「從SFDC流程刪除人員」動作。

>[!NOTE]
>
>僅在與Salesforce整合時可用。

1. 在資料庫中，按一下要從Salesforce中移除的人員。 然後按一下&#x200B;**[!UICONTROL 人員動作]**&#x200B;並選取&#x200B;**[!DNL Salesforce]**。

   ![](assets/delete-person-from-sfdc-1.png)

1. 選取&#x200B;**[!UICONTROL 從SFDC]**&#x200B;刪除人員。

   ![](assets/delete-person-from-sfdc-2.png)

1. 請確定Marketo **中的**&#x200B;刪除&#x200B;**[!UICONTROL false]**&#x200B;設定，然後按一下&#x200B;**[!UICONTROL 立即執行]**。

   ![](assets/delete-person-from-sfdc-3.png)

   在流程步驟執行後，您的人員將不再是Salesforce中的銷售機會，但將保留在Marketo中。

   >[!CAUTION]
   >
   >如果您將Marketo **中的**&#x200B;刪除設定為&#x200B;**[!UICONTROL true]**，並從Marketo中刪除人員和Salesforce的銷售機會，則為永久性刪除。 此動作無法還原。
