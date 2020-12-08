---
unique-page-id: 4720215
description: 在Wordpress Enterprise上實作RTP - Marketo Docs —— 產品檔案
title: Wordpress企業中RTP的實現
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# Wordpress企業中RTP的實現 {#implementing-rtp-on-wordpress-enterprise}

要實施RTP標籤，請遵循以下安裝說明：

1. 前往**帳戶設定。**

   1. 如果您已從「支援」收到JavaScript標籤，請繼續步驟3。\
      ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在「網域」下方，找出相關網域，然後按一下「 **產生標籤」**。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 複製RTP JavaScript標籤。
1. 以管理員使用者身分登入您的WordPress帳戶

   1. 在「 **外觀**」下，移至 **「自訂JavaScript**」。
   1. 將RTP Javascript標籤貼在現有代碼後面。

      ![](assets/image2014-12-3-17-3a51-3a46.png)
   >[!CAUTION]
   >
   >將代碼EXCLUDE貼上到以下標籤時：
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >    
   >僅插入指令碼本身。

1. 按一 **下更新**。
