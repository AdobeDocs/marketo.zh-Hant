---
unique-page-id: 11385053
description: 部署JavaScript for Content-AI —— 行銷檔案——產品檔案
title: 部署Content-AI適用的JavaScript
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# 部署Content-AI {#deploy-the-javascript-for-content-ai}適用的JavaScript

>[!NOTE]
>
>視購買日期而定，您的Marketo訂閱可能包含Marketo Predictive Content或Content`<sup>AI</sup>`。 對於使用預測性內容的使用者，Marketo會在2018年4月30日之前啟用「內容`<sup>AI</sup>`分析」功能。 若要將這些功能保留在該日期之後，請連絡您的Marketo Customer Success Manager以升級至Marketo Content`<sup>AI</sup>`。

若要使用預測性內容，您需要產生並設定RTP（Web個人化）`tag.`

## 產生標籤{#generate-tag}

1. 登入您的預測式內容帳戶。 前往&#x200B;**帳戶設定**。

   ![](assets/settings-dropdown-account-hands.png)

1. 在&#x200B;**域配置**&#x200B;中，找到相關域並按一下&#x200B;**生成標籤。**

   ![](assets/generate-tag.png)

1. 將「Web個人化」標籤複製並貼至您網站的HTML。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >複製「網頁個人化JavaScript」標籤，並貼為頁面標題中的第一個指令碼，位於`<head> </head>`標籤之間。 請參閱此處[實作指示的詳細說明](https://docs.marketo.com/display/docs/rtp+tag+implementation) [。](https://pages2.marketo.com/rtp-implementation.html)

1. 驗證標籤是否顯示在所有頁面上，包括著陸頁面和子網域。 請在`website’s`頁面上按一下滑鼠右鍵以檢查此項目。 前往Web瀏覽器中的「檢視頁面來源」**。**&#x200B;搜尋：「RTP」。
1. 確認「標籤」切換為「**ON**」。

