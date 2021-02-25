---
unique-page-id: 4720218
description: 使用Adobe Tag Manager - Marketo Docs —— 產品檔案實作RTP
title: 使用Adobe Tag Manager實作RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# 使用Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}實作RTP

要實施RTP標籤，請遵循以下安裝說明：

1. 登入您的RTP帳戶。

1. 前往&#x200B;**帳戶設定**。

   a.如果您已從「支援」收到JavaScript標籤，請繼續步驟4。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 在「Domain（域）」下，找到相關域，然後按一下「Generate Tag **（生成標籤**）」。

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. 登入您的動態標籤管理員帳戶([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in))。

1. 前往「**儀表板」。** 按一下相關的Web屬性。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. 前往&#x200B;**Rules**，按一下「建立新規則」。****

1. 填寫下列內容

   1. 名稱：**Marketo RTP**
   1. 條件（收合）:觸發規則位於- **頁面頂端**
   1. Javascript（收合）:按一下&#x200B;**添加新指令碼**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 呼叫新標籤：**Marketo RTP Tag**

1. 從RTP標籤中刪除以下代碼

   * `<script type='text/javascript'>`
   * `</script>`

1. 貼上RTP JavaScript標籤。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >請確定您移除所有標籤，並僅保留指令碼本身（無`<script type='text/javascript'>`、`</script>`）

1. 在指令碼編輯器中按一下「保存代碼」，在規則編輯器中按一下「保存規則」。********

1. 在「規則」面板中，找到Marketo RTP頁面載入規則，並在&#x200B;**Actions**&#x200B;下拉式清單中選取「啟動規則」**。**

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **驗** 證它是否顯示在所有頁面上，包括著陸頁面和子網域。

   您可以在網站的頁面上按一下滑鼠右鍵來完成。 前往&#x200B;**檢查元素**，按一下&#x200B;**網路**，搜尋：**RTP**。
