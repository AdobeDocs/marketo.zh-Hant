---
unique-page-id: 4720145
description: 使用Google Tag Manager實作RTP - Marketo檔案 — 產品檔案
title: 使用Google Tag Manager實作RTP
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 使用[!DNL Google Tag Manager]實作RTP {#implementing-rtp-using-google-tag-manager}

若要實作RTP標籤，請遵循下列安裝指示。

1. 登入您的[!DNL Google Tag Manager]帳戶。

1. 新增&#x200B;**[!UICONTROL Tag]** > **[!UICONTROL Tag Configurations]** > **[!UICONTROL Custom HTML Tag]。**&#x200B;呼叫它&#x200B;**RTP**。

1. 登入您的&#x200B;**RTP帳戶**。

1. 移至&#x200B;**[!UICONTROL Account Settings]**。

   a.如果您已經從「支援」收到JavaScript標籤，請繼續步驟6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在[!UICONTROL Domain]下，找到相關網域並按一下&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 複製RTP JavaScript標籤，並將其貼到您建立的新&#x200B;**自訂HTML標籤** （步驟1）。

1. 按一下&#x200B;**[!UICONTROL Add Rule to Fire Tag]**。 選擇「**[!UICONTROL All Pages]**」。

1. 按一下&#x200B;**[!UICONTROL Save]**&#x200B;並[發佈新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 確認其出現在所有頁面上，包括登陸頁面和子網域。

   a.您可以在網站的頁面上按一下滑鼠右鍵，以執行此操作。 移至&#x200B;**[!UICONTROL Inspect Element]**，搜尋&#x200B;**RTP**&#x200B;以找出標籤。
