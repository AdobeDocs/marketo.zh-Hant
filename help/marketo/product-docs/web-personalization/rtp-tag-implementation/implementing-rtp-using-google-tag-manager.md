---
unique-page-id: 4720145
description: 使用Google Tag Manager實作RTP - Marketo檔案 — 產品檔案
title: 使用Google Tag Manager實作RTP
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# 使用Google Tag Manager實作RTP {#implementing-rtp-using-google-tag-manager}

若要實作RTP標籤，請遵循下列安裝指示。

1. 登入您的Google Tag Manager帳戶。

1. 新增標籤>標籤設定>自訂HTML標籤**。**呼叫它 **RTP**.

1. 登入您的RTP帳戶**。**

1. 前往 **帳戶設定**.

   a.如果您已經從「支援」收到JavaScript標籤，請繼續步驟6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在「領域」下，找到相關領域並按一下 **產生標籤**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 複製RTP JavaScript標籤並將其貼到新的 **自訂HTML標籤** 您已建立（步驟1）。

1. 按一下 **+新增規則以引發標籤**. 選取 **所有頁面**.

1. 按一下 **儲存** 和 [發佈新版本](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. 確認它出現在所有頁面上，包括登陸頁面和子網域。

   a.您可以在網站的頁面上按一下滑鼠右鍵，即可完成此操作。 前往 **Inspect元素**，搜尋 **RTP** 以找出標籤。
