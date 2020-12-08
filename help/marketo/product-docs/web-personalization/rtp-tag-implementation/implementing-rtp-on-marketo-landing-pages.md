---
unique-page-id: 4720151
description: 在Marketo登陸頁面上實作RTP - Marketo Docs —— 產品檔案
title: Marketo登陸頁面上的RTP實現
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Marketo登陸頁面上的RTP實現 {#implementing-rtp-on-marketo-landing-pages}

要實施RTP標籤，請遵循以下安裝說明：

1. 前往 **Design Studio。** 開啟您要編輯的項目。 選擇「 **模板操作**」，選擇「編 **輯草稿」**

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 在「 **HTML來源」標籤上變更範本** 。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在您的RTP帳戶中，前往**帳戶設定。**

1. 如果您已從「支援」收到JavaScript標籤，請繼續步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在「網域」下方，找出相關網域，然後按一下「 **產生標籤」**。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 複製RTP JavaScript標籤並貼到標籤之間的所有著陸頁面范 **`<head> </head>`** 本。
1. 按一 **下「儲存** 」並 **關閉視窗** 。
1. 回到 **Design Studio**，從「範本動作」核准著陸頁面 **，按一下「核**&#x200B;準」 ****。\
   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後，您必須重新核 **準使用該範本的** ，範本變更才能生效。 您可以從主要「著陸頁面」區段一次重新核准所有項目。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 確認它出現在所有著 `pages including` 陸頁面和子網域。

   您可以按一下滑鼠右鍵來完成此 `website’s` 作業。 前往「檢 **視頁面來源」。** 搜尋 **RTP** ，以找出標籤。
