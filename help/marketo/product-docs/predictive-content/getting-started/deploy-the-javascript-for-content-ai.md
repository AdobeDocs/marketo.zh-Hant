---
unique-page-id: 11385053
description: 部署JavaScript for Content-AI - Marketo檔案 — 產品檔案
title: 部署Content-AI的JavaScript
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# 部署Content-AI的JavaScript {#deploy-the-javascript-for-content-ai}

若要使用預測性內容，您必須產生並設定RTP （網頁個人化）標籤。

## 產生標籤 {#generate-tag}

1. 登入您的預測性內容帳戶。 前往 **帳戶設定**.

   ![](assets/settings-dropdown-account-hands.png)

1. 在 **網域設定**，找到相關網域並按一下 **產生標籤**.

   ![](assets/generate-tag.png)

1. 將Web Personalization標籤複製並貼到網站的HTML中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >複製Web Personalization JavaScript標籤，並將其貼上為頁面標頭中的第一個指令碼，介於 `<head> </head>` 標籤之間。 檢視更多詳細資料 [此處為實作指示](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. 驗證標籤是否出現在所有頁面上，包括登陸頁面和子網域。 請在您網站的頁面上按一下滑鼠右鍵，以檢查此專案。 前往 **檢視頁面來源** 在網頁瀏覽器中。 搜尋： &#39;RTP&#39;。

1. 確認標籤切換設定為 **開啟**.
