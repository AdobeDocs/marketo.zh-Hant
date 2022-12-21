---
unique-page-id: 4720215
description: 在Wordpress Enterprise上實作RTP - Marketo檔案 — 產品檔案
title: 在Wordpress Enterprise上實現RTP
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# 在Wordpress Enterprise上實現RTP {#implementing-rtp-on-wordpress-enterprise}

若要實作您的RTP標籤，請遵循下列安裝指示：

1. 前往 **帳戶設定**.

   a.如果您已從「支援」收到JavaScript標籤，請繼續執行步驟3。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在「網域」下，找到相關網域並按一下 **產生標籤**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 複製RTP JavaScript標籤。

1. 以管理員使用者身分登入您的WordPress帳戶

   a.在 **外觀**，前往 **自訂JavaScript**.
b.將RTP Javascript標籤貼到現有程式碼的正後面。

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >將程式碼貼上為「排除」時，請執行下列標籤：
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >
   >僅插入指令碼本身。

1. 按一下 **更新**.
