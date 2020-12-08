---
unique-page-id: 7512454
description: 設定行動推播通知——行銷人員檔案——產品檔案
title: 設定行動推播通知
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# 設定行動推播通知 {#configure-mobile-push-notification}

1. 前往「行銷活動」區域。

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. 選取您的推播資產，然後按一下「 **編輯草稿**」。

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. 前往「設 **定」**。

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. 選取您想要的應用程式。 Android和Apple平台預設會啟用。

   ![](assets/image2016-8-23-16-3a53-3a33.png)

   如果您的推播訊息只套用至一個平台（例如iPhone的案例），則您可將其選取器滑入「停用」，以排除另一個平台。

   ![](assets/image2016-8-23-16-3a41-3a48.png)

   按一下「下一步」。

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. 輸入訊息文字或選取要新增Token的Token圖示。 然後，選取「點選 **動作」**。

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >如果平台已啟用，則會顯示在電話螢幕的左側。 在選取時，它會以顏色顯示。

   >[!NOTE]
   >
   >**定義**
   >
   >
   >有三種類型**點選動作：**
   >
   >
   >**啟動應用程式** -此應 **** 用程式會在點選通知時開啟您應用程式的首頁。 **自訂** (Custom)會使用深層連結來開啟您應用程式或您擁有連結之任何其他應用程式的其他區域(如需詳細資訊，請參閱 [下方的深層連結URI](#Deeplink) )。
   >
   >
   >**著陸頁面** -將您帶往指定的Marketo著陸頁面。
   >
   >
   >**外部URL** —— 將您帶至非Marketo登陸頁面。

   若要插入自訂點選動作的深層連結，請按一下「自訂」，然後在欄 [位中輸入深層連結URI](#Deeplink) 。

   ![](assets/image2016-7-28-16-3a19-3a13.png)

   若要插入Token，請選取Token，輸入預設值，然後按一下「插入」。

   >[!NOTE]
   >
   >Token會出現在您將游標置於文字方塊中的位置。 您可以使用多個Token。

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >訊息和點選動作在兩個平台上看起來都相同。

   僅適用於iOS，勾選核取方塊，讓應用程式在訊息送達時播放音效。 Android會自動播放音效。

   ![](assets/ios-tap-and-notification-hand.png)

   預覽其他平台，然後按一下「完成」。

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. 按一 **下「核准並關閉**」。

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

恭喜！ 現在推播通知已可供傳送。

## 深層連結URI {#deep-link-uris}

當訂閱者按一下推播訊息中的按鈕時，可以將按鈕帶到您應用程式的首頁，或直接帶到應用程式內的特定頁面。 深層連結是應用程式中特定頁面的唯一參考，看起來很像網站連結。

深層連結URI由三部分組成：方案名稱、路徑和識別碼。 在以下範例中，&quot;myappname&quot;是方案。 &quot;products&quot;是路徑，&quot;purple-shirt&quot;是識別碼。 當客戶點選時，會特別將他們帶到應用程式產品頁面中的紫色襯衫項目。

![](assets/image2016-7-29-12-3a49-3a1.png)

不過，您應用程式的深層連結結構可能與上述範例不同。 您的開發人員有許多定義深層連結URI的選項，因此請要求您的開發人員傳送您想要使用之頁面的URI（連結）給您。 這將確保您在推送訊息中輸入的URI指向正確位置。 您的開發人員可 [以在這裡找到更多資訊](http://developers.marketo.com/mobile/enabling-deep-links-in-your-app/)。

>[!NOTE]
>
>**相關文章**
>
>* [傳送行動推播通知](send-a-mobile-push-notification.md)

>



