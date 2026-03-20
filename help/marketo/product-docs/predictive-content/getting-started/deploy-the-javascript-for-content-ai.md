---
unique-page-id: 11385053
description: 瞭解如何產生並放置預測性內容的RTP Web Personalization標籤。 將其複製到您的頁首，驗證涵蓋範圍，並確認切換是否保持開啟。
title: 部署 Content-AI 適用的 JavaScript
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: cd7a000c415bedd561aa509e375ba0dee8e81d9f
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 8%

---

# 部署 Content-AI 適用的 JavaScript {#deploy-the-javascript-for-content-ai}

若要使用預測性內容，您需要產生並設定您的RTP （網頁Personalization）標籤。

## 產生標籤 {#generate-tag}

1. 登入您的預測性內容帳戶。 前往 **[!UICONTROL Account Settings]**。

   ![](assets/settings-dropdown-account-hands.png)

1. 在&#x200B;**[!UICONTROL Domain Configuration]**&#x200B;中，找到相關網域並按一下&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/generate-tag.png)

1. 將網頁Personalization標籤複製並貼到您網站的HTML中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >複製Web Personalization JavaScript標籤，並將其貼上為頁面標頭中的第一個指令碼，位於`<head> </head>`標籤之間。 請在此參閱更詳細的[實作指示](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)。

1. 確認標籤是否會出現在所有頁面上，包括登陸頁面和子網域。 請在您網站的頁面上按一下滑鼠右鍵，以勾選此選項。 在網頁瀏覽器中移至&#x200B;**[!UICONTROL View Page Source]**。 搜尋： &#39;RTP&#39;。

1. 確認標籤切換設定為&#x200B;**[!UICONTROL ON]**。
