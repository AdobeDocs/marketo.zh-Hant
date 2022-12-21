---
unique-page-id: 4720151
description: 在Marketo登陸頁面上實作RTP - Marketo檔案 — 產品檔案
title: 在Marketo登陸頁面上實作RTP
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# 在Marketo登陸頁面上實作RTP {#implementing-rtp-on-marketo-landing-pages}

若要實作您的RTP標籤，請遵循下列安裝指示：

1. 前往 **設計工作室。** 開啟要編輯的項目。 選擇 **範本動作**，選取 **編輯草稿**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 在 **HTML來源** 標籤。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在您的RTP帳戶中，前往 **帳戶設定**.

   a.如果您已從「支援」收到JavaScript標籤，請繼續執行步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在「網域」下，找到相關網域並按一下 **產生標籤**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 複製RTP JavaScript標籤，並貼到 **`<head> </head>`** 標籤。

1. 按一下 **儲存** 和 **關閉** 窗戶。

1. 回到 **Design Studio**，核准登錄頁面來自 **範本動作**，按一下 **核准**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後，你需要 **重新核准** 使用該範本的任何登錄頁面，範本皆會變更為生效。 您可以從主要登陸頁面區段一次重新核准所有項目。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 確認其顯示在所有頁面上，包括登陸頁面和子網域。

   若要這麼做，請以滑鼠右鍵按一下網站的頁面。 前往 **檢視頁面來源。** 搜尋 **RTP** 來尋找標籤。
