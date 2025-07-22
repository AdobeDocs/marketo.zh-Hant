---
unique-page-id: 4720149
description: 在Wordpress上實作RTP - Marketo檔案 — 產品檔案
title: 在Wordpress上實作RTP
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# 在[!DNL Wordpress]上實作RTP {#implementing-rtp-on-wordpress}

若要實作您的[!UICONTROL RTP tag]，請遵循下列安裝指示：

1. 開啟&#x200B;**佈景主題**&#x200B;的&#x200B;**[!DNL WordPress]header.php**&#x200B;檔案。

   您可以使用FTP使用者端存取您的伺服器，或直接從[!DNL WordPress]儀表板編輯您的主題檔案。 您的檔案編輯器位於側邊欄功能表的&#x200B;**[!UICONTROL Appearance]**&#x200B;標籤下方。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文字編輯器右側的範本檔案清單中，找到&#x200B;**header.php**&#x200B;並開啟它。

1. 移至&#x200B;**[!UICONTROL Account Settings]**。

   a.如果您已從支援部門收到JavaScript標籤 — 請繼續步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在[!UICONTROL Domain]下，找到相關網域並按一下&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 複製RTP JavaScript標籤，並將其貼到您的網站範本。

   a.確認這是頁面標頭處的第一個指令碼，介於&#x200B;**`<head> </head>`**&#x200B;個標籤之間。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 按一下&#x200B;**[!UICONTROL Update File]**&#x200B;以取得header.php檔案。

1. 確認其出現在所有頁面上，包括登陸頁面和子網域。

   a.您可以在網站的頁面上按一下滑鼠右鍵，以執行此操作。 移至&#x200B;**[!UICONTROL View Page Source]。**&#x200B;搜尋&#x200B;**RTP**&#x200B;以找出標籤。
