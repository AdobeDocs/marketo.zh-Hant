---
unique-page-id: 9437340
description: 使用Tealium Tag Manager - Marketo Docs —— 產品檔案實作RTP
title: 使用Tealium Tag Manager實現RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 使用Tealium Tag Manager實現RTP {#implementing-rtp-using-tealium-tag-manager}

要實施RTP標籤，請遵循以下安裝說明。

1. 登入您的Tealium Tag Manager帳戶。
1. 導覽至「標籤」標籤，並新增位於「標籤」市集「雜項」標籤下方的「標籤自訂容器標籤」。
1. 在「標題」欄位中，輸入 **Marketo RTP** ，然後按一 **下「完成」**。
1. 儲存您的變更。

   >[!NOTE]
   >
   >您還不需要發佈新容器。

1. 儲存描述檔後，按一下Tealium iQ主控台右上角的您的姓名／電子郵件地址。
1. 在「管理員」功能表中，按一下「 **帳戶管理員** 」下的「管理範本」。
1. 選取 **Tealium自訂容器：從下拉式清單** ，以開啟「標籤」範本的Marketo RTP。
1. 登入您的RTP帳戶。
1. 前往「帳戶設定」。

   >[!NOTE]
   >
   >如果您已從「支援」收到JavaScript標籤，請繼續步驟11。

1. 在「網域」下方，找出相關網域，然後按一下「 **產生標籤」**。
1. 複製RTP JavaScript標籤，並貼在Tealium描述檔範本的「開始標籤程式庫程式碼」和「結束標籤程式庫程式碼」之間。

   >[!NOTE]
   >
   >**重要步驟**
   >
   >從您置入 `<!-- RTP tag -->` 此檔 `<!-- End of RTP tag -->` 案的程式碼中移除和標籤。
   >
   >從您置入 `<script type='text/javascript'>` 此檔 `</script>` 案的程式碼中移除任何和標籤。

1. **按一下「儲存描述檔範本** 」，然後發佈您的新描述檔。

