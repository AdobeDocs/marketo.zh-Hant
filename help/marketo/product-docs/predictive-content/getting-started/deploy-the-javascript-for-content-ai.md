---
unique-page-id: 11385053
description: 部署JavaScript for Content-AI —— 行銷檔案——產品檔案
title: 部署Content-AI適用的JavaScript
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# 部署Content-AI {#deploy-the-javascript-for-content-ai}適用的JavaScript

若要使用預測性內容，您需要產生並設定RTP（Web個人化）標籤。

## 產生標籤{#generate-tag}

1. 登入您的預測式內容帳戶。 前往&#x200B;**帳戶設定**。

   ![](assets/settings-dropdown-account-hands.png)

1. 在&#x200B;**域配置**&#x200B;中，找到相關域並按一下&#x200B;**生成標籤**。

   ![](assets/generate-tag.png)

1. 將「Web個人化」標籤複製並貼至您網站的HTML。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >複製「網頁個人化JavaScript」標籤，並貼為頁面標題中的第一個指令碼，位於`<head> </head>`標籤之間。 請參閱此處[實作指示的詳細說明](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)。

1. 驗證標籤是否顯示在所有頁面上，包括著陸頁面和子網域。 在您網站的頁面上按一下滑鼠右鍵，以檢查此問題。 前往Web瀏覽器中的「檢視頁面來源」**。**&#x200B;搜尋：「RTP」。

1. 確認「標籤」切換為「**ON**」。
