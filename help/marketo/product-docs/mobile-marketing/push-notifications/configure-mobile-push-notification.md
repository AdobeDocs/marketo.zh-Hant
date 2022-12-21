---
unique-page-id: 7512454
description: 設定行動推播通知 — Marketo檔案 — 產品檔案
title: 設定行動推播通知
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 設定行動推播通知 {#configure-mobile-push-notification}

1. 前往 **行銷活動** 的上界。

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. 選取您的推送資產，然後按一下 **編輯草稿**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. 前往 **設定**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. 選取您想要的應用程式。 預設會啟用Android和Apple平台。

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. 如果您的推送訊息只套用至一個平台（例如iPhone的案例），則您可以將其選取器滑動至「停用」，以排除另一個平台。

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. 按一下 **下一個**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. 輸入訊息文字或選取Token圖示以新增Token。 然後，選取 **點選動作**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >如果平台已啟用，它會顯示在電話螢幕的左側。 選取後會以顏色顯示。

   >[!NOTE]
   >
   >點選動作有三種類型：
   >
   >**Launch應用程式** - **此應用** 在點選通知時開啟應用程式的首頁。 **自訂** 使用深層連結來開啟您應用程式或任何其他您擁有連結的應用程式的其他區域(請參閱 [深層連結URI](#Deeplink) 詳情請參閱下文)。
   >
   >**登陸頁面**  — 將您帶至指定的Marketo登陸頁面。
   >
   >**外部URL**  — 帶您前往非Marketo登陸頁面。

1. 若要插入自訂點選動作的深層連結，請按一下「自訂」，然後輸入 [深層連結URI](#Deeplink) 欄位。

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. 若要插入代號，請選取代號，輸入預設值，然後按一下「插入」。

   >[!NOTE]
   >
   >將游標置於文本框中的位置會顯示令牌。 您可以使用多個代號。

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >訊息和點選動作在兩種平台上看起來都一樣。

1. 僅限iOS，請核取核取方塊，告知應用程式在訊息到達時播放音效。 Android會自動播放音效。

   ![](assets/ios-tap-and-notification-hand.png)

1. 預覽其他平台，然後按一下 **完成**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. 按一下 **核准並關閉**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

恭喜您！現在推播通知已可供傳送。

## 深層連結URI {#deep-link-uris}

訂閱者按一下推送訊息中的按鈕時，可將其帶往您應用程式的首頁，或直接帶往應用程式內的特定頁面。 深層連結是您應用程式中特定頁面的唯一參考，看起來很像網站連結。

深層連結URI由三部分組成：配置名稱、路徑和標識符。 在以下範例中，「myappname」為配置。 路徑為&quot;products&quot;，而識別碼為&quot;purple-shirt&quot;。 當客戶點選時，會特別擷取至應用程式產品頁面中的紫色襯衫項目。

![](assets/image2016-7-29-12-3a49-3a1.png)

也就是說，您應用程式的深層連結結構可能與上述範例不同。 在定義深層連結URI時，您的開發人員有許多選項，因此請您的開發人員針對您想要使用的頁面，將URI（連結）傳送給您。 這將確保您在推送訊息中輸入的URI指向正確的位置。 您的開發人員可 [如需詳細資訊，請參閱這裡](https://developers.marketo.com/mobile/enabling-deep-links-in-your-app/).

>[!MORELIKETHIS]
>
>[傳送行動推播通知](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
