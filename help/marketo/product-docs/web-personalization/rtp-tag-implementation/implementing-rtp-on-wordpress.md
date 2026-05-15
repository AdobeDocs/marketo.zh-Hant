---
unique-page-id: 4720149
description: 瞭解如何在Marketo Engage中在wordpress上實施rtp，包括在dnl wordpress上實施rtp。 使用本指南完成您的下一個步驟。
title: 在 WordPress 上實施 RTP
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
TQID: https://experienceleague.adobe.com/5V3CEgasEJi4zrYoezh8Tt340VGHNNHaliF2wdbBLwY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 189
ht-degree: 3%

---

# 在[!DNL Wordpress]上實作RTP {#implementing-rtp-on-wordpress}

若要實作您的[!UICONTROL RTP tag]，請遵循下列安裝指示：

1. 開啟&#x200B;**[!DNL WordPress]佈景主題**&#x200B;的&#x200B;**header.php**&#x200B;檔案。

   您可以使用FTP使用者端存取您的伺服器，或直接從[!DNL WordPress]儀表板編輯您的主題檔案。 您的檔案編輯器位於側邊欄功能表的&#x200B;**[!UICONTROL Appearance]**&#x200B;標籤下方。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文字編輯器右側的範本檔案清單中，找到&#x200B;**header.php**&#x200B;並開啟它。

1. 前往 **[!UICONTROL Account Settings]**。

   答： 如果您已從支援部門收到JavaScript標籤 — 請繼續執行步驟5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在[!UICONTROL Domain]下，找到相關網域並按一下&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 複製RTP JavaScript標籤，並將其貼到您的網站範本。

   答： 請確定這是頁面標頭處的第一個指令碼，介於&#x200B;**`<head> </head>`**&#x200B;個標籤之間。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 按一下&#x200B;**[!UICONTROL Update File]**&#x200B;以取得header.php檔案。

1. 確認其出現在所有頁面上，包括登陸頁面和子網域。

   答： 若要這麼做，請在您網站的頁面上按一下滑鼠右鍵。 移至&#x200B;**[!UICONTROL View Page Source].** 搜尋&#x200B;**RTP**&#x200B;以找出標籤。
