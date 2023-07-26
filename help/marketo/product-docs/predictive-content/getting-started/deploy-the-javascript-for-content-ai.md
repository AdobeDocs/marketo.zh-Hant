---
unique-page-id: 11385053
description: 部署JavaScript for Content-AI - Marketo檔案 — 產品檔案
title: 為Content-AI部署JavaScript
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# 為Content-AI部署JavaScript {#deploy-the-javascript-for-content-ai}

若要使用預測性內容，您需要產生並設定您的RTP （網頁個人化）標籤。

## 產生標籤 {#generate-tag}

1. 登入您的預測性內容帳戶。 前往 **帳戶設定**.

   ![](assets/settings-dropdown-account-hands.png)

1. 在 **網域設定**，找到相關的網域，然後按一下 **產生標籤**.

   ![](assets/generate-tag.png)

1. 將Web Personalization標籤複製並貼到網站的HTML中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >複製Web Personalization JavaScript標籤，並將其貼上為頁面標頭中的第一個指令碼，介於 `<head> </head>` 標籤之間。 檢視更多詳情 [在此填入實作指示](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. 確認標籤是否會出現在所有頁面上，包括登陸頁面和子網域。 請在您網站的頁面上按一下滑鼠右鍵，以勾選此選項。 前往 **檢視頁面來源** 在網頁瀏覽器中。 搜尋： &#39;RTP&#39;。

1. 確認標籤切換設定為 **開啟**.
