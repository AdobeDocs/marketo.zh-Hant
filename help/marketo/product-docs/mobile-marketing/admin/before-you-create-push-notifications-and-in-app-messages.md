---
unique-page-id: 11376159
description: 建立推播通知和應用程式內訊息之前 — Marketo檔案 — 產品檔案
title: 建立推播通知和應用程式內訊息之前
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 建立推播通知和應用程式內訊息之前 {#before-you-create-push-notifications-and-in-app-messages}

建立推播通知和應用程式內訊息並不難，但您必須先準備好所有內容，才能開始使用。 Marketo管理員和行動應用程式開發人員應依照下列步驟準備必要的整合。

1. 首先，Marketo管理員 [新增行動應用程式](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. Marketo管理員 [傳送程式碼片段給開發人員](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. 開發人員下載SDK，並包含程式碼片段和其他方法， [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) 或 [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. 依預設，應用程式開啟時會觸發應用程式內訊息。 如果您想要觸發其他事件的訊息，例如在檢視特定頁面或按下特定按鈕時，開發人員需要將自訂事件新增至程式碼(請參閱 [應用程式內訊息的自訂事件](#CustomEvents) )。

1. 開發人員 [產生Android的伺服器API金鑰和專案編號](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) 或 [iOS的認證與密碼](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) 並傳送給Marketo管理員。

1. Marketo管理員會設定推播通知存取 [(Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) 或 [與憑證(iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Marketo管理員可輕鬆檢查是否已驗證您的推送設定。 快走 [此處](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## 應用程式內訊息的自訂事件 {#custom-events-for-in-app-messages}

若為應用程式內訊息，顯示觸發器會設為 **應用程式開啟** 依預設。 如果您想要使用任何自訂事件來觸發應用程式內訊息的顯示(例如 **按一下「新增至購物車」**, **檢視設定頁面**)、建立所需事件的清單，並提供給您的行動應用程式開發人員。 開發人員接著會將自訂事件新增至程式碼中。 核准後，在設定您的對象時，它們會顯示為顯示觸發器。 **注意**:自訂事件編碼核准程式可能需要一些時間才能完成。

完成應用程式內訊息和推播通知的所有準備工作後，該開始了！

>[!MORELIKETHIS]
>
>* [建立應用程式內訊息](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [建立推播通知](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

