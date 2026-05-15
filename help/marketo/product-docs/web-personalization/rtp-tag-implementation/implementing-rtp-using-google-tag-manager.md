---
unique-page-id: 4720145
description: 瞭解如何在Marketo Engage中使用Google標籤管理員實作rtp，包括使用dnl google實作rtp。 使用本指南完成您的下一個步驟。
title: 使用 Google Tag Manager 實施 RTP
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XesXGBf2aDsnsbS2Ro1RLdd1EVrj-mBdCiv8C0dj8NU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 152
ht-degree: 6%

---

# 使用[!DNL Google Tag Manager]實作RTP {#implementing-rtp-using-google-tag-manager}

若要實作RTP標籤，請遵循下列安裝指示。

1. 登入您的[!DNL Google Tag Manager]帳戶。

1. 新增&#x200B;**[!UICONTROL Tag]** > **[!UICONTROL Tag Configurations]** > **[!UICONTROL Custom HTML Tag].** 呼叫它&#x200B;**RTP**。

1. 登入您的&#x200B;**RTP帳戶**。

1. 前往 **[!UICONTROL Account Settings]**。

   答： 如果您已從支援部門收到JavaScript標籤，請繼續前往步驟6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在[!UICONTROL Domain]下，找到相關網域並按一下&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 複製RTP JavaScript標籤，並將其貼到您建立的新&#x200B;**自訂HTML標籤** （步驟1）。

1. 按一下「**[!UICONTROL Add Rule to Fire Tag]**」。 選取「**[!UICONTROL All Pages]**」。

1. 按一下&#x200B;**[!UICONTROL Save]**&#x200B;並[發佈新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 確認其出現在所有頁面上，包括登陸頁面和子網域。

   答： 若要這麼做，請在網站的頁面上按一下滑鼠右鍵。 移至&#x200B;**[!UICONTROL Inspect Element]**，搜尋&#x200B;**RTP**&#x200B;以找出標籤。
