---
unique-page-id: 4720149
description: 在Wordpress上實作RTP - Marketo Docs —— 產品檔案
title: 在Wordpress中實現RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---


# 在Wordpress上實現RTP {#implementing-rtp-on-wordpress}

要實施RTP標籤，請遵循以下安裝說明：

1. 開啟&#x200B;**WordPress主題**&#x200B;的&#x200B;**header.php**&#x200B;檔案。

   您可以使用FTP用戶端來存取您的伺服器，或直接從WordPress儀表板編輯您的主題檔案。 檔案編輯器位於側欄菜單的&#x200B;**Appearance**&#x200B;頁籤下。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文字編輯器右側的範本檔案清單中，尋找&#x200B;**header.php**&#x200B;並開啟它。

1. 前往&#x200B;**帳戶設定**。

   a.如果您已從「支援」收到JavaScript標籤，請繼續步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在「Domain（域）」下，找到相關域，然後按一下「Generate Tag **（生成標籤**）」。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 複製RTP JavaScript標籤並貼到您的網站範本。

   a.請確定它是頁首的第一個指令碼——介於&#x200B;**`<head> </head>`**&#x200B;標籤之間。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 按一下&#x200B;**更新檔案**&#x200B;作為header.php檔案。

1. 確認它出現在所有頁面，包括著陸頁面和子網域。

   a.您可以在網站的頁面上按一下滑鼠右鍵，以完成此作業。 前往&#x200B;**檢視頁面來源。** 搜索 **** RTP以查找標籤。
