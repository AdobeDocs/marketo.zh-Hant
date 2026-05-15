---
unique-page-id: 14745655
description: 瞭解如何讓Sales Connect使用者看到Marketo行銷活動。 共用行銷活動，讓賣家可以從Sales Connect新增銷售機會。
title: 讓 Sales Connect 使用者可以看到行銷活動
exl-id: 1fde53e3-2764-4e4b-897f-635b78534133
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/WdSLwrvoXF6L4jID6HThIn2JST-aDvtPtXAoWqJO7ZI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 14%

---

# 讓[!DNL Sales Connect]個使用者看到行銷活動 {#make-a-campaign-visible-to-sales-connect-users}

行銷活動只有在顯示後才可共用。 以下說明該怎麼做。

1. 選取（或建立）您要共用的行銷活動。

   ![](assets/make-a-marketing-campaign-visible-msc-1.png)

1. 按一下「**[!UICONTROL Smart List]**」索引標籤。

   ![](assets/make-a-marketing-campaign-visible-msc-2.png)

1. 新增[!UICONTROL Campaign is Requested]觸發器。

   ![](assets/make-a-marketing-campaign-visible-msc-3.png)

1. 針對來源，請選擇[!UICONTROL is] **[!UICONTROL Web Service API]**。

   ![](assets/make-a-marketing-campaign-visible-msc-4.png)

1. 按一下「**[!UICONTROL Flow]**」索引標籤。

   ![](assets/make-a-marketing-campaign-visible-msc-5.png)

1. 新增[!UICONTROL Interesting Moment]流程動作。

   ![](assets/make-a-marketing-campaign-visible-msc-6.png)

1. 針對 [!UICONTROL Type]，請選取 **[!UICONTROL Web]**。

   ![](assets/make-a-marketing-campaign-visible-msc-7.png)

1. 在[!UICONTROL Description]方塊中，寫訊息給您的銷售團隊。 在此範例中，我們使用代號來指定已填寫的表單。

   ![](assets/make-a-marketing-campaign-visible-msc-8.png)

1. 按一下「**[!UICONTROL Schedule]**」標籤，然後&#x200B;**[!UICONTROL Activate]**&#x200B;促銷活動。

   ![](assets/make-a-marketing-campaign-visible-msc-9.png)
