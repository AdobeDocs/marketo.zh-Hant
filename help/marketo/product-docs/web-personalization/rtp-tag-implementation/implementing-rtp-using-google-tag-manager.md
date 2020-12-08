---
unique-page-id: 4720145
description: 使用Google Tag Manager - Marketo Docs —— 產品檔案實作RTP
title: 使用Google Tag Manager實現RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 0%

---


# 使用Google Tag Manager實現RTP {#implementing-rtp-using-google-tag-manager}

要實施RTP，請遵 `tag please` 循以下安裝說明。

1. 登入您的Google標籤管理員帳戶。

1. 新增「標籤>標籤設定>自訂HTML標籤**」。**叫它 **RTP**。

1. 登入您的RTP帳戶**。**

1. 前往**帳戶設定。**

   1. 如果您已從「支援」收到JavaScript標籤，請繼續步驟6。

      ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在「網域」下方，找出相關網域，然後按一下「 **產生標籤」**。

   ** ![](assets/image2014-11-30-15-3a20-3a17.png)

   **

1. 複製RTP JavaScript標籤並貼至您建立的新 **自訂HTML標籤** （步驟1）。

1. 按一 **下+新增規則至觸發標籤**。 選取 **所有頁面**。

1. 按一下**儲存**並 [發佈新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 確認它出現在所有著 `pages, including` 陸頁面和子網域。

   1. 您可以在頁面上按一下滑鼠右鍵，以完成此 `website’s` 作業。 前往**Inspect Element。 **搜尋**RTP **以找出標籤。

