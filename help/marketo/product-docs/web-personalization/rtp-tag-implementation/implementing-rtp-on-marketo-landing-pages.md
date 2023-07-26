---
unique-page-id: 4720151
description: 在Marketo登陸頁面上實作RTP - Marketo檔案 — 產品檔案
title: 在Marketo登陸頁面上實作RTP
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# 在Marketo登陸頁面上實作RTP {#implementing-rtp-on-marketo-landing-pages}

若要實作RTP標籤，請遵循下列安裝指示：

1. 前往 **Design Studio。** 開啟要編輯的專案。 選取 **範本動作**，選取 **編輯草稿**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 變更範本於 **HTML來源** 標籤。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在您的RTP帳戶中，移至 **帳戶設定**.

   a.如果您已從支援部門收到JavaScript標籤 — 請繼續步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在「網域」下，找到相關網域並按一下 **產生標籤**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 複製RTP JavaScript標籤，並將其貼到您的所有登入頁面範本中 **`<head> </head>`** 標籤之間。

1. 按一下 **儲存** 和 **關閉** 視窗。

1. 返回 **Design Studio**，核准以下位置的登陸頁面： **範本動作**，按一下 **核准**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後，您需要 **重新核准** 使用該範本作為範本的任何登入頁面都會變更以生效。 您可以一次從主要登入頁面區段重新核准所有頁面。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 確認其出現在所有頁面上，包括登陸頁面和子網域。

   若要這麼做，請在您網站的頁面上按一下滑鼠右鍵。 前往 **檢視頁面來源。** 搜尋 **RTP** 以找出標籤。
