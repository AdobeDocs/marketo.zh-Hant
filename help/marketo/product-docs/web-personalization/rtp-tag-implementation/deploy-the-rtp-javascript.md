---
unique-page-id: 4719332
description: 瞭解如何在Marketo Engage中部署rtp javascript，包括部署rtp javascript。 使用本指南完成您的下一個步驟。
title: 部署 RTP JavaScript
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XUylNa8clUib-aMhpAR8fjeu4pHRA8KSQydSH1AVxF8
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
source-wordcount: 171
ht-degree: 5%

---

# 部署 RTP JavaScript {#deploy-the-rtp-javascript}

若要產生和設定您的RTP標籤，請遵循下列安裝指示

## [!UICONTROL Generate Tag] {#generate-tag}

1. 登入您的RTP帳戶。 前往 **[!UICONTROL Account Settings]**。

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. 在&#x200B;**[!UICONTROL Domain]**&#x200B;和&#x200B;**[!UICONTROL Domain Configuration]**&#x200B;中，找到相關網域並按一下&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. 將網頁Personalization (RTP)標籤複製並貼到您的網站中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >複製RTP JavaScript標籤，並將其貼上為頁面標頭中的第一個指令碼，介於`<head> </head>`個標籤之間。

   請確定標籤出現在所有頁面上，包括登陸頁面和子網域。 請在您網站的頁面上按一下滑鼠右鍵，以勾選此選項。 前往在網頁瀏覽器中檢視頁面Source 。 搜尋： &#39;RTP&#39;。

1. [!UICONTROL Tag]切換設定為&#x200B;**[!UICONTROL ON]**。

   確認[!UICONTROL Tag]切換設定為[!UICONTROL ON]。 您應該會開始看到資料流入組織的標籤。

   您現在已經設定好RTP標籤，可以開始[建立區段](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)和即時行銷活動！

1. 確認標籤位於所有頁面上。
