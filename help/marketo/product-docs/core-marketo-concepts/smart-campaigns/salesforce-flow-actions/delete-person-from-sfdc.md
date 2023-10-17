---
unique-page-id: 1147031
description: 從SFDC刪除人員 — Marketo檔案 — 產品檔案
title: 從SFDC刪除人員
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 從SFDC刪除人員 {#delete-person-from-sfdc}

如果您需要從Salesforce移除特定銷售機會集，但保留為Marketo Engage中的人員，則可使用「從SFDC流程刪除人員」動作。

>[!NOTE]
>
>僅在與Salesforce整合時可用。

1. 在資料庫中，按一下要從Salesforce中移除的人員。 然後按一下 **[!UICONTROL 個人動作]** 並選取 **[!DNL Salesforce]**.

   ![](assets/person-actions-salesforce.png)

1. 選取 **[!UICONTROL 從SFDC刪除人員]**.

   ![](assets/delete-person-from-sfdc.png)

1. 請確定 **[!UICONTROL 在Marketo中刪除]** 設定為 **[!UICONTROL false]**，然後按一下 **[!UICONTROL 立即執行]**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   在流程步驟執行後，您的人員將不再是Salesforce中的銷售機會，但將保留在Marketo中。

   >[!CAUTION]
   >
   >如果您設定 **[!UICONTROL 在Marketo中刪除]** 至 **[!UICONTROL true]** 並刪除Marketo中的人員和Salesforce中的銷售機會，則永遠消失。 此動作無法還原。
