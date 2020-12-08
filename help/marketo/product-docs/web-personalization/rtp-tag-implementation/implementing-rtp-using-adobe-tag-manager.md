---
unique-page-id: 4720218
description: 使用Adobe Tag Manager - Marketo Docs —— 產品檔案實作RTP
title: 使用Adobe Tag Manager實作RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# 使用Adobe Tag Manager實作RTP {#implementing-rtp-using-adobe-tag-manager}

要實施RTP標籤，請遵循以下安裝說明：

1. 登入您的RTP帳戶。
1. 前往「帳 **戶設定」。**

   如果您已從「支援」收到JavaScript標籤，請繼續步驟4。

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. 在「網域」下方，找出相關網域，然後按一下「 **產生標籤」**。

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. 登入您的動態標籤管理員帳戶([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in))。
1. 前往「控制 **面板」。** 按一下相關的Web屬性。

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. 前往「規 **則」,** 按一 **下「建立新規則」。**

1. 填寫下列內容

   1. 名稱： **Marketo RTP**
   1. 條件（收合）:觸發規則位 **於——頁面頂端**
   1. Javascript（收合）:按一 **下新增指令碼**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. 呼叫新標籤： **Marketo RTP標籤**
1. 從RTP標籤中刪除以下代碼

   * `<script type='text/javascript'>`
   * `</script>`

1. 貼上RTP JavaScript標籤。

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >請確定您移除所有標籤，並僅保留指令碼本身( `<script type='text/javascript'>` no, `</script>` )

1. 按一 **下指令碼編輯器中的「儲存代碼** 」，以及規則 **編輯器中的「儲存規則** 」。

1. 在「規則」面板中，找出Marketo RTP頁面載入規則，並在「動作」下拉式清單中選 **取** 「啟 **動規則」**。

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **確認它** 出現在所有頁面上，包括著陸頁面和子網域。

   您可以在網站的頁面上按一下滑鼠右鍵來完成。 前往「 **檢查元素**」，按一下「**網路」、「**搜尋： **RTP**。
