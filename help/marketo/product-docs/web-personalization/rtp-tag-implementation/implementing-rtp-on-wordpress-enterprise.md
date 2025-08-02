---
unique-page-id: 4720215
description: 在Wordpress Enterprise上實作RTP - Marketo檔案 — 產品檔案
title: 在Wordpress Enterprise上實作RTP
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '95'
ht-degree: 1%

---

# 在Wordpress Enterprise上實作RTP {#implementing-rtp-on-wordpress-enterprise}

若要實作您的[!UICONTROL RTP tag]，請遵循下列安裝指示：

1. 移至&#x200B;**[!UICONTROL Account Settings]**。

   a.如果您已從支援部門收到JavaScript標籤 — 請繼續步驟3。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在[!UICONTROL Domain]下，找到相關網域並按一下&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 複製RTP JavaScript標籤。

1. 以管理員使用者身分登入您的[!DNL WordPress]帳戶

   a.在&#x200B;**[!UICONTROL Appearance]**&#x200B;底下，移至&#x200B;**[!UICONTROL Custom JavaScript]**。
b.將RTP Javascript標籤貼到現有程式碼的正後方。

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >貼上程式碼時，請排除下列標籤：
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >僅插入指令碼本身。

1. 按一下「**[!UICONTROL Update]**」。
