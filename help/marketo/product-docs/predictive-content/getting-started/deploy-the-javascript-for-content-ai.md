---
unique-page-id: 11385053
description: 部署JavaScript for Content-AI —— 行銷檔案——產品檔案
title: 部署Content-AI適用的JavaScript
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# 部署Content-AI適用的JavaScript {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>根據購買日期，您的Marketo訂閱可能包含Marketo預測性內容或內容`<sup>AI</sup>`。 對於使用「預測性內容」的使用者，Marketo會在2018年4月`<sup>AI</sup>` 30日之前啟用「內容分析」功能。 若要將這些功能保留在該日期之後，請連絡您的Marketo Customer Success Manager以升級至Marketo Content`<sup>AI</sup>`。

若要使用預測性內容，您需要產生並設定RTP（網路個人化） `tag.`

## 產生標籤 {#generate-tag}

1. 登入您的預測式內容帳戶。 前往「帳 **戶設定」**。

   ![](assets/settings-dropdown-account-hands.png)

1. 在「 **網域設定**」中，找出相關網域，然後按一下「 **產生標籤」。**

   ![](assets/generate-tag.png)

1. 將「Web個人化」標籤複製並貼至您網站的HTML。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >複製「網頁個人化JavaScript」標籤，並貼為頁面標題中的第一個指令碼，在標籤之間 `<head> </head>` 切換。 請參閱此處的 [更詳細的實作指示](http://docs.marketo.com/display/docs/rtp+tag+implementation)[。](http://pages2.marketo.com/rtp-implementation.html)

1. 驗證標籤是否顯示在所有頁面上，包括著陸頁面和子網域。 請在您的頁面上按一下滑鼠右鍵以檢 `website’s` 查此項。 前往Web **瀏覽器中的** 「檢視頁面來源」。 搜尋：「RTP」。
1. 確認「標籤」切換為 **ON**。

