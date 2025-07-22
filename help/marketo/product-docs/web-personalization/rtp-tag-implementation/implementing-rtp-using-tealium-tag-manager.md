---
unique-page-id: 9437340
description: 使用Tealium Tag Manager實作RTP - Marketo檔案 — 產品檔案
title: 使用Tealium Tag Manager實作RTP
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 1%

---

# 使用[!DNL Tealium]標籤管理員實作RTP {#implementing-rtp-using-tealium-tag-manager}

若要實作RTP標籤，請遵循下列安裝指示。

1. 登入您的[!DNL Tealium]標籤管理員帳戶。

1. 導覽至[!UICONTROL Tags]標籤，然後新增[!UICONTROL Tealium Custom Container Tag]，該標籤位於標籤市集的[!UICONTROL Misc]標籤下方。

1. 在[!UICONTROL Title field]中，輸入&#x200B;**Marketo RTP**&#x200B;並按一下&#x200B;**[!UICONTROL Finish]**。

1. 儲存您的變更。

   >[!NOTE]
   >
   >目前不需要發佈新容器。

1. 儲存設定檔後，按一下Tealium iQ主控台右上角的姓名/電子郵件地址。

1. 在[!UICONTROL Admin]功能表上，按一下&#x200B;**[!UICONTROL Manage Templates]**&#x200B;底下的[!UICONTROL Account Admin]。

1. 從下拉式清單中選取&#x200B;**[!UICONTROL Tealium Custom Container]： Marketo RTP**&#x200B;以開啟Tag範本。

1. 登入您的RTP帳戶。

1. 移至[!UICONTROL Account Settings]。

   >[!NOTE]
   >
   >如果您已從支援部門收到JavaScript標籤，請繼續前往步驟11。

1. 在[網域]下，找到相關網域，然後按一下&#x200B;**[!UICONTROL Generate Tag]**。

1. 複製RTP JavaScript標籤，並將其貼到您的Tealium設定檔範本中[!UICONTROL Start Tag Library Code]到[!UICONTROL End Tag Library Code]之間。

   >[!NOTE]
   >
   >**重要步驟**
   >
   >從您放置在此檔案中的程式碼移除`<!-- RTP tag -->`和`<!-- End of RTP tag -->`標籤。
   >
   >從您放置在此檔案中的程式碼移除任何`<script type='text/javascript'>`和`</script>`標籤。

1. 按一下&#x200B;**[!UICONTROL Save Profile Template]**&#x200B;並發佈您的新設定檔。
