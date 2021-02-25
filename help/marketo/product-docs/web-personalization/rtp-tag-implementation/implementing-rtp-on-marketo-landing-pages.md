---
unique-page-id: 4720151
description: 在Marketo登陸頁面上實作RTP - Marketo Docs —— 產品檔案
title: Marketo登陸頁面上的RTP實現
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# 在Marketo登陸頁面上實現RTP {#implementing-rtp-on-marketo-landing-pages}

要實施RTP標籤，請遵循以下安裝說明：

1. 前往&#x200B;**Design Studio。** 開啟您要編輯的項目。選擇&#x200B;**模板操作**，選擇&#x200B;**編輯草稿**。

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 在&#x200B;**HTML Source**&#x200B;標籤上變更範本。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在RTP帳戶中，轉至&#x200B;**Account Settings**。

   a.如果您已從「支援」收到JavaScript標籤，請繼續步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在「Domain（域）」下，找到相關域，然後按一下「Generate Tag **（生成標籤**）」。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 複製RTP JavaScript標籤並貼到&#x200B;**`<head> </head>`**&#x200B;標籤之間的所有著陸頁面範本。

1. 按一下「保存&#x200B;**」和「關閉**&#x200B;窗口」。****

1. 回到&#x200B;**Design Studio**&#x200B;中，從&#x200B;**範本動作**&#x200B;核准著陸頁面，按一下&#x200B;**批准**。

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後，您需要&#x200B;**重新核准**&#x200B;使用該範本的任何著陸頁面，讓範本變更生效。 您可以從主要「著陸頁面」區段一次重新核准所有項目。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 確認它出現在所有頁面，包括著陸頁面和子網域。

   您可以在網站的頁面上按一下滑鼠右鍵，以完成此作業。 前往&#x200B;**檢視頁面來源。** 搜索 **** RTP以查找標籤。
