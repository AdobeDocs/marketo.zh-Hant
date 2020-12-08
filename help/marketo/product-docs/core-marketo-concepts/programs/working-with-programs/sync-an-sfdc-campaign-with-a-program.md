---
unique-page-id: 1147154
description: 將SFDC促銷活動與計畫同步——行銷人員文檔——產品文檔
title: 將SFDC促銷活動與計畫同步
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# 將SFDC促銷活動與計畫同步 {#sync-an-sfdc-campaign-with-a-program}

Marketo可讓您將程式與Salesforce促銷活動同步，以維護兩個系統中的相同人員清單，包括其狀態。 開始吧！

>[!NOTE]
>
>**必要條件**
>
>您必須先啟 [用Salesforce促銷活動同步](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) 。

>[!CAUTION]
>
>當將SFDC促銷活動與Marketo計畫同步時，對於計畫的子促銷活動，隱含的SFDC動作（例如，添加到SFDC促銷活動，同步到SFDC）將被禁用。

1. 前往行 **銷活動**。

   ![](assets/login-marketing-activities-1.png)

1. 選擇您的方案。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 按一 **下「方案動作**」，然後選 **取「Salesforce促銷活動同步」**。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 選擇**建立新**或選擇現有的Salesforce促銷活動。

   >[!TIP]
   >
   >如果您選取現有的Salesforce促銷活動，請確 [定符合Salesforce促銷活動和Marketo程式的程式狀態](../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)。

1. 輸入新促銷活動的名稱，然後按一下「 **儲存**」。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 現在，您可以在方案摘要頁面中驗證促銷活動同步詳細資訊。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   太棒了！ 現在，Marketo中的任何計畫狀態變更都會同步至SFDC促銷活動，反之亦然。

