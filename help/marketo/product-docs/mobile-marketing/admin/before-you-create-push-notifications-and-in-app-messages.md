---
unique-page-id: 11376159
description: 在您建立推播通知和應用程式內訊息之前——行銷人員檔案——產品檔案
title: 建立推播通知和應用程式內訊息之前
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---


# 建立推播通知和應用程式內訊息之前{#before-you-create-push-notifications-and-in-app-messages}

建立推播通知和應用程式內訊息並不困難，但您必須先準備好一切，才能開始。 行銷人員和行動應用程式開發人員應依照下列步驟來準備必要的整合。

1. 首先，行銷人員管理員[新增行動應用程式](add-a-mobile-app.md)
1. Marketo Admin接著[傳送程式碼片段給開發人員](send-sdk-code-to-a-developer.md)
1. 開發人員會下載SDK，並包含[Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/)或[iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)的程式碼片段和其他方法
1. 依預設，應用程式開啟時會觸發應用程式內訊息。 如果您想要觸發其他事件的訊息，例如在檢視特定頁面或推送特定按鈕時，開發人員需要將自訂事件新增至程式碼（請參閱下方的「應用程式內訊息的自訂事件」[）](#CustomEvents)
1. 開發人員[會產生Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/)或[的伺服器API金鑰和專案編號，並傳送給行銷人員管理員](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/)
1. 行銷人員管理員使用伺服器API金鑰(Android)](configure-mobile-app-android-push-access.md)或使用憑證(iOS)](configure-mobile-app-ios-push-access.md)設定推播通知存取[[

>[!TIP]
>
>行銷人員管理員可輕鬆檢查您的推播設定是否經過驗證。 只要前往[這裡](verify-push-configuration.md)即可。

## 應用程式內訊息的自訂事件{#custom-events-for-in-app-messages}

對於應用程式內傳訊，預設會將顯示觸發器設為&#x200B;**App Open**。 如果您想要使用任何自訂事件來觸發應用程式內訊息的顯示（例如，**「點按新增至購物車」**、**「檢視設定頁面」**），請建立所需事件清單，並將它提供給您的行動應用程式開發人員。 然後，開發人員會將自訂事件新增至程式碼。 在核准後，在設定您的觀眾時，會以顯示觸發器的形式顯示。 **注意**:自訂事件編碼核准程式可能需要一些時間才能完成。

完成應用程式內訊息和推播通知的所有準備後，就該開始了！

>[!MORELIKETHIS]
>
>* [建立應用程式內訊息](https://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [建立推播通知](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



