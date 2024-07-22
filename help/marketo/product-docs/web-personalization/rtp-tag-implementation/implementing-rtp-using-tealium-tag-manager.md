---
unique-page-id: 9437340
description: 使用Tealium Tag Manager實作RTP - Marketo檔案 — 產品檔案
title: 使用Tealium Tag Manager實作RTP
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# 使用Tealium Tag Manager實作RTP {#implementing-rtp-using-tealium-tag-manager}

若要實作RTP標籤，請遵循下列安裝指示。

1. 登入您的Tealium Tag Manager帳戶。

1. 導覽至「標籤」標籤，然後新增Tealium自訂容器標籤，該標籤位於「標籤」市場的「雜項」標籤下方。

1. 在[標題]欄位中，輸入&#x200B;**Marketo RTP**，然後按一下[完成]****。

1. 儲存您的變更。

   >[!NOTE]
   >
   >目前不需要發佈新容器。

1. 儲存設定檔後，按一下Tealium iQ主控台右上角的姓名/電子郵件地址。

1. 在[管理]功能表上，按一下[帳戶管理]下的[管理範本] ****。

1. 從下拉式清單中選取&#x200B;**Tealium自訂容器： Marketo RTP**&#x200B;以開啟Tag範本。

1. 登入您的RTP帳戶。

1. 前往「帳戶設定」。

   >[!NOTE]
   >
   >如果您已從支援部門收到JavaScript標籤，請繼續前往步驟11。

1. 在[網域]下，找到相關網域，然後按一下[產生標籤]。****

1. 複製RTP JavaScript標籤，並將其貼到您Tealium設定檔範本的「開始標籤程式庫代碼」和「結束標籤程式庫代碼」之間。

   >[!NOTE]
   >
   >**重要步驟**
   >
   >從您放置在此檔案中的程式碼移除`<!-- RTP tag -->`和`<!-- End of RTP tag -->`標籤。
   >
   >從您放置在此檔案中的程式碼移除任何`<script type='text/javascript'>`和`</script>`標籤。

1. **按一下[儲存設定檔範本]**&#x200B;並發佈您的新設定檔。
