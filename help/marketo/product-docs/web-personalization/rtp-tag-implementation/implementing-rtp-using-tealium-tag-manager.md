---
unique-page-id: 9437340
description: 使用Tealium Tag Manager - Marketo Docs —— 產品檔案實作RTP
title: 使用Tealium Tag Manager實現RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 使用Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}實現RTP

要實施RTP標籤，請遵循以下安裝說明。

1. 登入您的Tealium Tag Manager帳戶。

1. 導覽至「標籤」標籤，並新增位於「標籤」市集「雜項」標籤下方的「標籤自訂容器標籤」。

1. 在「標題」欄位中，輸入&#x200B;**Marketo RTP** ，然後按一下&#x200B;**完成**。

1. 儲存您的變更。

   >[!NOTE]
   >
   >您還不需要發佈新容器。

1. 儲存描述檔後，按一下Tealium iQ主控台右上角的您的姓名／電子郵件地址。

1. 在「管理」功能表上，按一下「帳戶管理」下的「管理範本」。****

1. 選擇&#x200B;**Tealium自訂容器：從下拉式清單中將Marketo RTP**&#x200B;開啟「標籤」範本。

1. 登入您的RTP帳戶。

1. 前往「帳戶設定」。

   >[!NOTE]
   >
   >如果您已從「支援」收到JavaScript標籤，請繼續步驟11。

1. 在「Domain（域）」下，找到相關域，然後按一下「Generate Tag **（生成標籤**）」。

1. 複製RTP JavaScript標籤，並貼在Tealium描述檔範本的「開始標籤程式庫程式碼」和「結束標籤程式庫程式碼」之間。

   >[!NOTE]
   >
   >**重要步驟**
   >
   >從您置入此檔案的程式碼中移除`<!-- RTP tag -->`和`<!-- End of RTP tag -->`標籤。
   >
   >從您置入此檔案的程式碼中移除任何`<script type='text/javascript'>`和`</script>`標籤。

1. **按一下「儲存描述檔范** 本」，然後發佈您的新描述檔。
