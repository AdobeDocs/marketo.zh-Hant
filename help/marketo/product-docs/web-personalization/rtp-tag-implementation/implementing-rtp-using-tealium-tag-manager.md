---
unique-page-id: 9437340
description: 使用Tealium Tag Manager實作RTP - Marketo檔案 — 產品檔案
title: 使用Tealium Tag Manager實作RTP
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# 使用Tealium Tag Manager實作RTP {#implementing-rtp-using-tealium-tag-manager}

若要實作您的RTP標籤，請遵循下列安裝指示。

1. 登入您的Tealium Tag Manager帳戶。

1. 導覽至「標籤」標籤，並新增「標籤自訂容器標籤」，位於「標籤」市集的「雜項」標籤下。

1. 在標題欄位中，輸入 **Marketo RTP** 按一下 **完成**.

1. 儲存您的變更。

   >[!NOTE]
   >
   >還不需要發佈新容器。

1. 儲存設定檔後，按一下Tealium iQ主控台右上角的您的姓名/電子郵件地址。

1. 在「管理」功能表中，按一下 **管理範本** 在「帳戶管理員」下。

1. 選擇 **範本自訂容器：Marketo RTP** 從下拉式清單中開啟「標籤」範本。

1. 登入您的RTP帳戶。

1. 前往「帳戶設定」。

   >[!NOTE]
   >
   >如果您已從「支援」收到JavaScript標籤，請繼續進行步驟11。

1. 在「網域」下，找到相關網域並按一下 **產生標籤**.

1. 複製RTP JavaScript標籤，並在範本設定檔範本的開始標籤程式庫程式碼和結束標籤程式庫程式碼之間貼上。

   >[!NOTE]
   >
   >**重要步驟**
   >
   >移除 `<!-- RTP tag -->` 和 `<!-- End of RTP tag -->` 標籤。
   >
   >移除任何 `<script type='text/javascript'>` 和 `</script>` 標籤。

1. **按一下「儲存設定檔範本」** 並發佈您的新設定檔。
