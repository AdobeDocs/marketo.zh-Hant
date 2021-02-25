---
unique-page-id: 4720215
description: 在Wordpress Enterprise上實作RTP - Marketo Docs —— 產品檔案
title: Wordpress企業中RTP的實現
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# 在Wordpress Enterprise上實現RTP{#implementing-rtp-on-wordpress-enterprise}

要實施RTP標籤，請遵循以下安裝說明：

1. 前往&#x200B;**帳戶設定**。

   a.如果您已從「支援」收到JavaScript標籤，請繼續步驟3。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在「Domain（域）」下，找到相關域，然後按一下「Generate Tag **（生成標籤**）」。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 複製RTP JavaScript標籤。

1. 以管理員使用者身分登入您的WordPress帳戶

   a.在&#x200B;**Appearance**&#x200B;下，轉至&#x200B;**Custom JavaScript**。
b.將RTP Javascript標籤貼在現有代碼後面。

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

1. 按一下&#x200B;**Update**。
