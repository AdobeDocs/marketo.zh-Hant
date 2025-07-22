---
unique-page-id: 11376159
description: 建立推播通知和應用程式內訊息之前 — Marketo檔案 — 產品檔案
title: 建立推播通知和應用程式內訊息之前
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 建立推播通知和應用程式內訊息之前 {#before-you-create-push-notifications-and-in-app-messages}

建立推播通知和應用程式內訊息並不困難，但您需要先準備好所有專案，然後才能開始。 Marketo管理員和行動應用程式開發人員應依照下列步驟，準備必要的整合。

1. 首先，Marketo管理員[新增行動應用程式](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md)。

1. Marketo管理員接著[傳送程式碼片段給開發人員](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md)。

1. 開發人員下載適用於[Android](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)或[iOS](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios)的SDK，並包含程式碼片段和其他方法。

1. 依預設，應用程式會在開啟時觸發應用程式內訊息。 如果您想要觸發其他事件的訊息，例如檢視特定頁面或按一下特定按鈕時，開發人員需要將自訂事件新增至程式碼（請參閱下方的[應用程式內訊息的自訂事件](#CustomEvents)）。

1. 開發人員[會產生Android的伺服器API金鑰和專案編號](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)或[iOS的憑證和密碼](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios)，並將其傳送給Marketo管理員。

1. Marketo管理員使用伺服器API金鑰(Android) [設定推播通知存取](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md)，或使用憑證(iOS) [設定](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md)。

>[!TIP]
>
>Marketo管理員可輕鬆檢視推播設定是否已驗證。 只要[這裡](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md)。

## 應用程式內訊息的自訂事件 {#custom-events-for-in-app-messages}

對於應用程式內傳訊，顯示觸發程式預設為&#x200B;**[!UICONTROL App Open]**。 如果您想要使用任何自訂事件來觸發應用程式內訊息的顯示（例如，**按一下[加入購物車]**、**檢視設定頁面**），請建立所需事件的清單，並將清單提供給您的行動應用程式開發人員。 開發人員會將自訂事件新增至程式碼中。 在核准後，在設定您的對象時，它們會顯示為顯示觸發器。 **警告**：自訂事件編碼核准程式可能需要一些時間才能完成。

應用程式內訊息和推播通知的準備工作全部完成後，您就可以開始了！

>[!MORELIKETHIS]
>
>* [建立應用程式內訊息](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [建立推播通知](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
