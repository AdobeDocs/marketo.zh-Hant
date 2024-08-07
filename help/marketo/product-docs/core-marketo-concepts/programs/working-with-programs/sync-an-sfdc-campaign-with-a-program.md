---
unique-page-id: 1147154
description: 將SFDC促銷活動與程式同步 — Marketo檔案 — 產品檔案
title: 將SFDC促銷活動與程式同步
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# 將SFDC促銷活動與程式同步 {#sync-an-sfdc-campaign-with-a-program}

Marketo Engage可讓您將方案與[!DNL Salesforce]行銷活動同步，以維持兩個系統中的相同人員清單，包括其狀態。 讓我們開始吧！

>[!PREREQUISITES]
>
>您必須先[啟用 [!DNL Salesforce] 行銷活動同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}。

>[!CAUTION]
>
>將SFDC促銷活動與Marketo Engage方案同步時，針對方案的子促銷活動，隱含的SFDC動作（例如，新增至SFDC促銷活動、同步至SFDC）將會停用。

1. 移至&#x200B;**[!UICONTROL 行銷活動]**。

   ![](assets/login-marketing-activities-1.png)

1. 選取您的程式。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 按一下&#x200B;**[!UICONTROL 程式動作]**，然後選取&#x200B;**[!UICONTROL Salesforce Campaign同步]**。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 選取&#x200B;**[!UICONTROL 新建]**&#x200B;或選擇現有的[!DNL Salesforce]行銷活動。

   >[!TIP]
   >
   >如果您選取現有的[!DNL Salesforce]行銷活動，請確定[符合 [!DNL Salesforce] 行銷活動的方案狀態和Marketo方案](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}。

1. 輸入新行銷活動的名稱，然後按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 現在您可以在方案摘要頁面中驗證Campaign同步處理詳細資料。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   太好了！ 現在，Marketo中的任何方案狀態變更都會同步至SFDC行銷活動，反之亦然。
