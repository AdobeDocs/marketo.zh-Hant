---
unique-page-id: 11376159
description: 建立推播通知和應用程式內訊息之前 — Marketo檔案 — 產品檔案
title: 建立推播通知和應用程式內訊息之前
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 建立推播通知和應用程式內訊息之前 {#before-you-create-push-notifications-and-in-app-messages}

建立推播通知和應用程式內訊息並不困難，但您需要先準備好所有專案，然後才能開始。 Marketo管理員和行動應用程式開發人員應遵循下列步驟，準備必要的整合。

1. 首先，Marketo管理員 [新增行動應用程式](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. Marketo管理員，然後 [傳送程式碼片段給開發人員](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. 開發人員會下載SDK，並包含適用於的程式碼片段和其他方法 [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) 或 [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. 依預設，應用程式開啟時會觸發應用程式內訊息。 如果您想要觸發其他事件的訊息，例如檢視特定頁面或按下特定按鈕時，開發人員需要將自訂事件新增至程式碼(請參閱 [應用程式內訊息的自訂事件](#CustomEvents) 下)。

1. 開發人員 [為Android產生伺服器API金鑰和專案編號](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) 或 [iOS的認證和密碼](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) 並傳送給Marketo管理員。

1. Marketo管理員會設定推播通知存取權 [使用伺服器API金鑰(Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) 或 [使用憑證(iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Marketo管理員可輕鬆檢視您的推送設定是否已驗證。 立即執行 [此處](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## 應用程式內訊息的自訂事件 {#custom-events-for-in-app-messages}

若為應用程式內傳訊，顯示觸發器會設為 **應用程式開啟** 依預設。 如果您想要使用任何自訂事件來觸發應用程式內訊息的顯示(例如， **點按新增到購物車**， **檢視設定頁面**)，建立所需事件清單，然後將其提供給您的行動應用程式開發人員。 開發人員隨後會將自訂事件新增至程式碼中。 在核准後，在設定您的對象時，它們會顯示為顯示觸發器。 **注意**：自訂事件編碼核准程式可能需要一些時間才能完成。

應用程式內訊息和推播通知的所有準備工作完成後，您就可以開始了！

>[!MORELIKETHIS]
>
>* [建立應用程式內訊息](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [建立推播通知](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
