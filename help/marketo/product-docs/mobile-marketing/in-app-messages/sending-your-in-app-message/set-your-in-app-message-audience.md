---
unique-page-id: 10617431
description: 設定應用程式內訊息對象 — Marketo檔案 — 產品檔案
title: 設定您的應用程式內訊息對象
exl-id: 696ae5b6-7063-41bc-bcef-27879182ff1e
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 1%

---

# 設定您的應用程式內訊息對象 {#set-your-in-app-message-audience}

第一個步驟是決定應該接收您應用程式內訊息的使用者。 您必須設定智慧清單。

1. 按一下「**[!UICONTROL Edit Smart List]**」。

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. 在「智慧列示」中，**[!UICONTROL Has Mobile App Activity]**&#x200B;觸發程式會自動填入。 按一下下拉式清單，然後選取您要放置訊息的應用程式。

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >應用程式內訊息程式目前不支援行動應用程式欄位的多個值。

1. **[!UICONTROL App Open]**&#x200B;是預設的「動作」設定，但您可以選取任何已設定的自訂事件。

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >預設觸發器([!UICONTROL App Open])和開發人員新增至程式碼的任何自訂觸發器會自動顯示在[!UICONTROL Action]選擇器中。 如果缺少自訂事件，請洽詢您的開發人員，確認他們已將自訂事件新增至應用程式。 請注意，自訂事件編碼和核准程式可能需要一些時間才能完成。 如需詳細資訊，請參閱[本文章](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md)。

1. 有需要的話，**[!UICONTROL Has Mobile App Activity]**&#x200B;觸發程式可以使用限制。

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. 您可以將篩選器新增至智慧清單，以限制接收應用程式內訊息的使用者。 在此範例中，使用&#x200B;**[!UICONTROL Acquisition Date]**&#x200B;篩選時，只有在2016年6月9日取得的人會傳送應用程式內訊息。

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. 返回您的應用程式內訊息「控制面板」。 在下拉式清單中設定顯示限制。

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >預設顯示限製為&#x200B;**[!UICONTROL Once per session]**。 如果您要在收件者回覆後停止顯示訊息，請選取&#x200B;**[!UICONTROL Every time until tapped]**。 如果每次都應該顯示，無論收件者做什麼，請選取&#x200B;**[!UICONTROL Every time]**。

   ![](assets/image2016-5-9-15-3a32-3a6.png)

做得很好！您已設定好您的對象。 您已取得藍色長條和綠色勾號。

[選取您的應用程式內訊息](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md)的時間！
