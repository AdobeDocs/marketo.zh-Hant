---
unique-page-id: 11378869
description: 建立瀏覽器SMS訊息 — Marketo檔案 — 產品檔案
title: 建立瀏覽器SMS訊息
exl-id: 9ec0da97-7a80-4c40-be79-be08d7d1d9c1
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 建立瀏覽器SMS訊息 {#create-a-vibes-sms-message}

以下說明如何建立Vibes SMS訊息。

>[!AVAILABILITY]
>
>此功能是您Adobe Marketo Engage帳戶的附加元件。 為了正確布建，必須透過Adobe購買。 如需詳細資訊，請聯絡Adobe帳戶團隊（您的客戶經理）。

>[!NOTE]
>
>SMS文本消息傳送不符合HIPAA。

1. 前往 **行銷活動** 並按一下右鍵程式。

   ![](assets/mobile-right-click-hand.jpg)

1. 按一下 **新本機資產**.

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >或者，您也可以按一下 **新增** 下拉式清單。

1. 按一下 **SMS訊息**.

   ![](assets/new-local-asset-selection-hand.jpg)

1. 輸入新SMS訊息的名稱和可選說明，然後按一下 **建立**.

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. 按一下 **編輯草稿**.

   ![](assets/edit-draft-hand.jpg)

1. 在訊息編輯器中，按一下藍色泡泡內部，然後開始輸入文字。

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >美國和加拿大的限制不同，分別為160和130個字元。 如果超過這些字元限制，您的訊息可能會遭到分割。 雖然我們會顯示您何時超過加拿大限制，但編輯器會針對美國進行最佳化，並根據美國限制來分割訊息。

1. 按一下 **代號** 在「插入」功能表中，將代號新增至訊息。

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >新增代號可能會導致訊息超過字元限制。 然後訊息會分割，導致額外費用。

1. 按一下 **連結** 在「插入」功能表中，將連結新增至訊息。

   ![](assets/full-message-link-hand.jpg)

1. 選取連結類型。 Marketo著陸頁面為預設值。 若您執行此動作，則需從下拉式清單中選取登錄頁面，然後按一下 **插入**.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >預設會選取兩個追蹤連結。

1. 如果您想改用外部URL，請按一下 **外部URL** 按鈕，然後在URL欄位中輸入URL。 按一下 **插入**.

   ![](assets/insert-link-url-hands.jpg)

1. 連結會顯示在訊息中。

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo會顯示品牌追蹤網域的連結預覽。 如果清除了mkt_tok連結核取方塊，連結會變更。 同時清除「追蹤連結」核取方塊，URL將縮短為其基本長度(例如，www.mygooglepage.com)。

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >字元計數只會反映最低訊息中包含的字元。

如果插入的內容超過美國限制，編輯器會將您的訊息分成若干區段。 絕對總數限制為900個字元。 達到上限後，訊息傳送至其對象時，訊息會自動截斷。
