---
unique-page-id: 4720149
description: 在Wordpress上實作RTP - Marketo檔案 — 產品檔案
title: 在Wordpress上實作RTP
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 在Wordpress上實作RTP {#implementing-rtp-on-wordpress}

若要實作RTP標籤，請遵循下列安裝指示：

1. 開啟&#x200B;**WordPress佈景主題**&#x200B;的&#x200B;**header.php**&#x200B;檔案。

   您可以使用FTP使用者端存取伺服器，或直接從WordPress儀表板編輯您的主題檔案。 您的檔案編輯器位於側邊欄功能表的&#x200B;**外觀**&#x200B;標籤下。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文字編輯器右側的範本檔案清單中，找到&#x200B;**header.php**&#x200B;並開啟它。

1. 移至&#x200B;**帳戶設定**。

   a.如果您已從支援部門收到JavaScript標籤 — 請繼續步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在[網域]下，找到相關網域，然後按一下[產生標籤]。**&#x200B;**

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 複製RTP JavaScript標籤，並將其貼到您的網站範本。

   a.確認這是頁面標頭處的第一個指令碼，介於&#x200B;**`<head> </head>`**&#x200B;個標籤之間。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 按一下&#x200B;**更新檔案**&#x200B;以取得header.php檔案。

1. 確認其出現在所有頁面上，包括登陸頁面和子網域。

   a.您可以在網站的頁面上按一下滑鼠右鍵，以執行此操作。 前往&#x200B;**檢視頁面Source。**&#x200B;搜尋&#x200B;**RTP**&#x200B;以找出標籤。
