---
unique-page-id: 4720218
description: 使用Adobe Tag Manager實作RTP - Marketo檔案 — 產品檔案
title: 使用Adobe Tag Manager實作RTP
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 使用Adobe Tag Manager實作RTP {#implementing-rtp-using-adobe-tag-manager}

若要實作RTP標籤，請遵循下列安裝指示：

1. 登入您的RTP帳戶。

1. 移至&#x200B;**帳戶設定**。

   a.如果您已從支援部門收到JavaScript標籤 — 請繼續步驟4。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 在[網域]下，找到相關網域，然後按一下[產生標籤]。****

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. 登入您的動態標籤管理員帳戶([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in))。

1. 前往&#x200B;**儀表板。**&#x200B;按一下相關的Web屬性。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. 移至&#x200B;**規則**，按一下&#x200B;**建立新規則**。

1. 填寫下列內容

   1. 名稱： **Marketo RTP**
   1. 條件（摺疊） ：觸發規則於 — **頁面頂端**
   1. Javascript （摺疊）：按一下&#x200B;**新增指令碼**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 呼叫新標籤： **Marketo RTP標籤**

1. 從RTP標籤中移除下列程式碼

   * `<script type='text/javascript'>`
   * `</script>`

1. 貼上RTP JavaScript標籤。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >請確定您移除所有標籤，並只留下指令碼本身（無`<script type='text/javascript'>` ， `</script>` ）

1. 在指令碼編輯器中按一下&#x200B;**儲存程式碼**，在規則編輯器中按一下&#x200B;**儲存規則**。

1. 在「規則」面板中，找出Marketo RTP頁面載入規則，並在「**動作**」下拉式清單中選取「**啟用規則**」。

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **驗證**&#x200B;它是否出現在所有頁面，包括登陸頁面和子網域。

   您可以在網站的頁面上按一下滑鼠右鍵，以執行此操作。 移至&#x200B;**Inspect元素**，按一下&#x200B;**網路**，搜尋： **RTP**。
