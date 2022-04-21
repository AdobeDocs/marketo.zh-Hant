---
description: 將動態聊天連接到Marketo-Marketo文檔 — 產品文檔
title: 將動態聊天連接到Marketo
exl-id: bad6c2dc-d4e7-4f98-bf6d-743043f96e4e
source-git-commit: 9b49c9f0ee03ab72672f46618fb24eed174bf835
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# 將動態聊天連接到Marketo {#connect-dynamic-chat-to-marketo}

在您完成 [初始設定](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md)，是時候執行一次同步，將動態聊天連接到您的Marketo訂閱。

1. 在「我的Marketo」中，按一下 **動態聊天** 平鋪。

   ![](assets/connect-dynamic-chat-to-marketo-1.png)

   >[!NOTE]
   >
   >如果看不到磁貼，請聯繫您的Marketo管理員。

1. 如果您以前曾與Adobe ID聯繫過應用程式，您將直接轉到動態聊天。 如果沒有， [設定你的Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html)。

1. 要連接您的Marketo實例，請選擇 **整合**。

   ![](assets/connect-dynamic-chat-to-marketo-2.png)

1. 在Marketo卡上，按一下 **啟動同步**。

   ![](assets/connect-dynamic-chat-to-marketo-3.png)

1. 從您的Marketo實例中最多選擇50個標準或自定義欄位以同步到動態聊天，以用於受眾目標、資料映射和個性化。 按一下 **下一個** 完成。

   ![](assets/connect-dynamic-chat-to-marketo-4.png)

   >[!CAUTION]
   >
   >此時，屬性選擇 **不能** 在初始同步後更改。 完成同步後，您只能返回並添加更多內容（如果選擇的數量少於50）。

1. 複查您的選擇(提醒：無法在同步後刪除屬性，因此按一下 **編輯選擇** 如果需要更改此步驟中的任何內容)。 按一下 **確認** 完成啟動同步。

   ![](assets/connect-dynamic-chat-to-marketo-5.png)

>[!NOTE]
>
>同步可能需要2到24小時的任意時間完成，具體取決於資料庫的大小。

## 連結您的Adobe組織和Marketo {#link-your-adobe-org-and-marketo}

接下來，是時候把Adobe和Marketo聯繫起來了。

1. 登錄到 [experience.adobe.com](https://experience.adobe.com)。

1. 在Experience Cloud中的任何位置按一下螢幕，然後按ctrl+i。在 **分配的組織** 頁籤，突出顯示並複製組織ID(_減_ 「@AdobeOrg」)。 按 **關閉** 完成。

   ![](assets/connect-dynamic-chat-to-marketo-6.png)

1. 在Marketo，轉到 **管理** 選擇 **Adobe組織映射**。

   ![](assets/connect-dynamic-chat-to-marketo-7.png)

1. 按一下 **編輯**。

   ![](assets/connect-dynamic-chat-to-marketo-8.png)

1. 貼上在步驟2中複製的組織ID並按一下 **確定**。

   ![](assets/connect-dynamic-chat-to-marketo-9.png)

>[!MORELIKETHIS]
>
>[初始設定](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md)
