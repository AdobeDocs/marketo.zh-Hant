---
unique-page-id: 4720149
description: 在Wordpress上實作RTP - Marketo檔案 — 產品檔案
title: 在Wordpress上實作RTP
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# 在Wordpress上實作RTP {#implementing-rtp-on-wordpress}

若要實作您的RTP標籤，請遵循下列安裝指示：

1. 開啟 **header.php** 檔案 **WordPress主題**.

   您可以使用FTP用戶端存取伺服器，或直接從WordPress控制面板編輯主題檔案。 檔案編輯器位於 **外觀** 標籤。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文字編輯器右側的範本檔案清單中，尋找 **header.php** 然後開啟它。

1. 前往 **帳戶設定**.

   a.如果您已從「支援」收到JavaScript標籤，請繼續執行步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在「網域」下，找到相關網域並按一下 **產生標籤**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 複製RTP JavaScript標籤並貼到您的網站範本。

   a.請確定這是頁首的第一個指令碼 — 介於 **`<head> </head>`** 標籤。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 按一下 **更新檔案** （用於header.php檔案）。

1. 確認其顯示在所有頁面上，包括登陸頁面和子網域。

   a.若要這麼做，請以滑鼠右鍵按一下網站的頁面。 前往 **檢視頁面來源。** 搜尋 **RTP** 來尋找標籤。
