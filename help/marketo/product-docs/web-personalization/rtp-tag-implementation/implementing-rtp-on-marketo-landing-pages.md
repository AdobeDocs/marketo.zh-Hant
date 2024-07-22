---
unique-page-id: 4720151
description: 在Marketo登陸頁面上實作RTP - Marketo檔案 — 產品檔案
title: 在Marketo登陸頁面上實作RTP
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# 在Marketo登陸頁面上實作RTP {#implementing-rtp-on-marketo-landing-pages}

若要實作RTP標籤，請遵循下列安裝指示：

1. 前往&#x200B;**設計工作室。**&#x200B;開啟您要編輯的專案。 選取&#x200B;**範本動作**，選取&#x200B;**編輯草稿**。

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 在&#x200B;**HTMLSource**&#x200B;標籤上進行範本變更。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在您的RTP帳戶中，移至&#x200B;**帳戶設定**。

   a.如果您已從支援部門收到JavaScript標籤 — 請繼續步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在[網域]下，找到相關網域，然後按一下[產生標籤]。****

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 複製RTP JavaScript標籤，並將其貼到&#x200B;**`<head> </head>`**&#x200B;標籤之間的所有登陸頁面範本中。

1. 按一下&#x200B;**儲存**&#x200B;並&#x200B;**關閉**&#x200B;視窗。

1. 返回&#x200B;**Design Studio**，核准來自&#x200B;**範本動作**&#x200B;的登入頁面，按一下&#x200B;**核准**。

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後，您需要&#x200B;**重新核准**&#x200B;使用該範本的任何登入頁面，範本變更才會生效。 您可以一次從主要登入頁面區段重新核准所有頁面。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 確認其出現在所有頁面上，包括登陸頁面和子網域。

   若要這麼做，請在您網站的頁面上按一下滑鼠右鍵。 前往&#x200B;**檢視頁面Source。**&#x200B;搜尋&#x200B;**RTP**&#x200B;以找出標籤。
