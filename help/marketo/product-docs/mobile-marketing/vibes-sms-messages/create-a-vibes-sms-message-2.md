---
description: 建立Vibes SMS訊息 — Marketo檔案 — 產品檔案
title: 建立Vibes SMS訊息
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# 建立Vibes SMS訊息 {#create-a-vibes-sms-message}

以下說明如何建立Vibes SMS訊息。

>[!AVAILABILITY]
>
>此功能可作為您的Adobe Marketo Engage帳戶的附加元件使用。 為了適當地布建，您必須透過Adobe購買。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。

1. 前往 **行銷活動**.

   ![](assets/mobile-right-click-hand.jpg)

1. 以滑鼠右鍵按一下方案，然後選取 **新增本機資產**.

   ![](assets/mobile-right-click-hand.jpg)

1. 按一下 **新增本機資產**.

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >或者，您可以按一下 **新增** 下拉式清單。

1. 按一下 **簡訊訊息**.

   ![](assets/new-local-asset-selection-hand.jpg)

1. 輸入新SMS訊息的名稱和說明（選用），然後按一下 **建立**.

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. 按一下 **編輯草稿**.

   ![](assets/edit-draft-hand.jpg)

1. 在訊息編輯器中，在藍色泡泡內按一下，並開始輸入文字。

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >使用標準ASCII字元集時，SMS訊息的字元限製為160個字元。 如果超過160個字元，訊息將會根據字元總數進行分割。

1. 按一下 **Token** 在「插入」功能表中新增Token至訊息。

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >新增Token可能會造成訊息超過字元限制。 然後，會分割訊息，導致其他訊息。

   >[!IMPORTANT]
   >
   >SMS法規遵循：所有輸出SMS訊息都必須包含品牌名稱或程式說明。 對於循環訊息程式，每個訂閱者應每月至少提供一次HELP和STOP指示。

   ??????使用Marketo URL縮短程式將導致您的訊息??????案中使用X個字元

1. 按一下 **連結** 在「插入」功能表中，將連結新增至訊息。

   ![](assets/full-message-link-hand.jpg)

1. 選取連結型別。 預設值為「Marketo登陸頁面」。 如果您這麼做，您必須從下拉式清單中選取登入頁面，然後按一下 **插入**.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >* 預設會選取這兩個追蹤連結。
   >* 使用Marketo URL縮短程式會導致訊息中使用X個字元。??????????????????

1. 如果您想改用外部URL，請按一下 **外部URL** 按鈕，並在URL欄位中輸入URL。 按一下 **插入**.

   ![](assets/insert-link-url-hands.jpg)

   >[!CAUTION]
   >
   >建議用於 _非_ 使用URL縮短程式（例如Bitly），因為電信業者可能會將您的訊息標示為垃圾訊息。

1. 連結會顯示在訊息中。

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo會顯示品牌追蹤網域的連結預覽。 如果您清除mkt_tok連結核取方塊，則連結會變更。 也清除追蹤連結核取方塊，URL會縮短至其基本長度(例如www.mygooglepage.com)。

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >字元計數僅反映最低訊息中包含的字元。

如果您插入的訊息超過美國的限制，編輯器會將您的訊息分成多個區段。 900個字元的絕對總限製為。 達到此限制後，訊息在傳送給其對象時將會自動截斷。

美國限制????????
