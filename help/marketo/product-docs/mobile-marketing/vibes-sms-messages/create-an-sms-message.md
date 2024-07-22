---
description: 建立SMS訊息 — Marketo檔案 — 產品檔案
title: 建立簡訊訊息
feature: Mobile Marketing
exl-id: 94749ea4-2fe3-4d90-9b31-35700ddd1670
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 建立簡訊訊息 {#create-an-sms-message}

以下說明如何建立SMS訊息。

>[!AVAILABILITY]
>
>此功能可作為您的Adobe Marketo Engage帳戶的附加元件使用。 為了適當地布建，您必須透過Adobe購買。 如需詳細資訊，請聯絡Adobe客戶團隊（您的客戶經理）。 Marketo Vibes SMS原生整合在美國和加拿大提供。 對於其他國家/地區，透過Marketo Webhook的連線可透過[直接連絡Vibes](https://www.vibes.com/talk-to-sales)來使用。

>[!PREREQUISITES]
>
>[將Vibes新增為LaunchPoint Service](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}

1. 移至&#x200B;**[!UICONTROL 行銷活動]**。

   ![](assets/create-an-sms-message-1.png)

1. 用滑鼠右鍵按一下所需的程式，然後選取&#x200B;**[!UICONTROL 新增本機資產]**。

   ![](assets/create-an-sms-message-2.png)

1. 選取&#x200B;**簡訊訊息**。

   ![](assets/create-an-sms-message-3.png)

1. 輸入新SMS訊息的名稱和選擇性說明，然後按一下[建立]。****

   ![](assets/create-an-sms-message-4.png)

1. 在編輯器中，在藍色泡泡內按一下，並開始輸入文字。

   ![](assets/create-an-sms-message-5.png)

   >[!NOTE]
   >
   >使用標準ASCII字元集時，SMS訊息的字元限製為160個字元。 如果超過160個字元，訊息將會根據字元總數進行分割。

1. 若要在訊息中新增權杖，請撰寫快速問候語，然後按一下&#x200B;**權杖**。

   ![](assets/create-an-sms-message-6.png)

   >[!NOTE]
   >
   >新增Token可能會造成訊息超過字元限制。 接著會分割訊息，並建立其他訊息。

   >[!IMPORTANT]
   >
   >SMS法規遵循：所有輸出SMS訊息都必須包含品牌名稱或程式說明。 對於循環訊息程式，每個訂閱者應每月至少提供一次HELP和STOP指示。

1. 選取所需的&#x200B;**Token**，輸入選擇性的&#x200B;**預設值**，然後按一下&#x200B;**建立**。

   ![](assets/create-an-sms-message-7.png)

1. 若要新增連結，請選取訊息中您希望其出現的位置，然後按一下[連結]。****

   ![](assets/create-an-sms-message-8.png)

1. 選取連結型別。 預設值為「Marketo登陸頁面」。 如果您這麼做，請按一下「著陸頁面」下拉式清單，然後選取所需頁面。 完成時，按一下&#x200B;**插入**。

   ![](assets/create-an-sms-message-9.png)

   >[!NOTE]
   >
   >預設會選取這兩個追蹤連結。 取消勾選「僅包含mkt_tok 」仍可追蹤連結，但在重新導向後，目的地URL將不會包含mkt_tok查詢字串引數。 此引數由Marketo登陸頁面和Munchkin使用，以確保正確追蹤人員活動（例如人員選擇退出時）。

1. 如果您想改用外部URL，請選取&#x200B;**外部URL**，輸入/貼上URL，然後按一下&#x200B;**插入**。

   ![](assets/create-an-sms-message-10.png)

   >[!NOTE]
   >
   >保留「追蹤連結」選取狀態時，Marketo會自動修改URL以進行追蹤。 如果您選擇停用追蹤，則未變更的訊息中將會顯示URL （例如`www.adobe.com`）。

   >[!CAUTION]
   >
   >建議&#x200B;_不_&#x200B;使用URL縮短程式（例如Bitly），因為電信業者可能會將您的訊息標示為垃圾訊息。

1. 連結會顯示在訊息中。

   ![](assets/create-an-sms-message-11.png)

   >[!NOTE]
   >
   >Marketo會顯示品牌追蹤網域的連結預覽。 如果您清除mkt_tok連結核取方塊，則連結會變更。

如果您插入超過160個字元，編輯器會將您的SMS分成多個區段。 每則訊息的整體限製為900個字元。 如果超過此值，訊息在傳送時將截斷。
