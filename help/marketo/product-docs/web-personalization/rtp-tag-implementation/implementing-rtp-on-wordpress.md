---
unique-page-id: 4720149
description: 在Wordpress上實作RTP - Marketo Docs —— 產品檔案
title: 在Wordpress中實現RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# 在Wordpress中實現RTP {#implementing-rtp-on-wordpress}

要實施RTP標籤，請遵循以下安裝說明：

1. 開啟 **WordPress主題的header** .php **檔案**。

   您可以使用FTP用戶端來存取您的伺服器，或直接從WordPress儀表板編輯您的主題檔案。 檔案編輯器位於側欄菜單的「 **Appearance** （外觀）」頁籤下。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文字編輯器右側的範本檔案清單中，尋找 **header.php** ，然後開啟它。
1. 前往「帳 **戶設定」。**

   如果您已從「支援」收到JavaScript標籤，請繼續步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在「網域」下方，找出相關網域，然後按一下「 **產生標籤」**。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 複製RTP JavaScript標籤並貼到您的網站範本。

   請確定這是頁首的第一個指令碼——介於標籤之 **`<head> </head>`** 間。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 按一下 **標頭。php檔案的** 「更新檔案」。
1. 確認它出現在所有著 `pages including` 陸頁面和子網域。

   您可以按一下滑鼠右鍵來完成此 `website’s` 作業。 前往「檢 **視頁面來源」。** 搜尋 **RTP** ，以找出標籤。
