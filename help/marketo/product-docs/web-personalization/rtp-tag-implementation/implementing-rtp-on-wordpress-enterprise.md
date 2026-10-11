---
unique-page-id: 4720215
description: 瞭解如何在Marketo Engage中在wordpress enterprise上實施rtp，包括在wordpress上實施rtp。 使用本指南完成您的下一個步驟。
title: 在 WordPress Enterprise 上實施 RTP
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/S0LvRrD1V6hkWN5L5TlnoaIqcDvXLjfm5do2-1WQTNw'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 13%
---
# 在 WordPress Enterprise 上實施 RTP {#implementing-rtp-on-wordpress-enterprise}

若要實作您的[!UICONTROL RTP tag]，請遵循下列安裝指示：

1. 前往 **[!UICONTROL Account Settings]**。

   答： 如果您已從支援部門收到JavaScript標籤 — 請繼續執行步驟3。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在[!UICONTROL Domain]下，找到相關網域並按一下&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 複製RTP JavaScript標籤。

1. 以管理員使用者身分登入您的[!DNL WordPress]帳戶

   答： 在&#x200B;**[!UICONTROL Appearance]**&#x200B;底下，移至&#x200B;**[!UICONTROL Custom JavaScript]**。
   b. 將RTP Javascript標籤貼到現有程式碼的正後方。

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
