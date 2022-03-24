---
description: 電子郵件跟蹤概述 — Marketo文檔 — 產品文檔
title: 電子郵件跟蹤概述
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 電子郵件跟蹤概述 {#email-tracking-overview}

## 回復跟蹤的工作原理 {#how-reply-tracking-works}

回復跟蹤是通過查看您發送的每封電子郵件中的郵件ID來完成的。 每封電子郵件都包含一個唯一的郵件ID，它允許我們進行一些最佳回復跟蹤。

>[!PREREQUISITES]
>
>與電子郵件伺服器的連接：Sales Connect必須與您的收件箱連接，以便我們知道何時收到新答復。 您需要將Sales Connect帳戶連接到Gmail。 如果您使用Outlook，我們需要與您的exchange伺服器整合。

如果Sales Connect無法跟蹤潛在客戶對您的電子郵件的回復，則它將無法基於回複檢測或記錄回復到Salesforce的市場活動。 什麼是說任何電子郵件地址都可以回復？

這意味著，如果您發電子郵件至flynn@flynnsarcade.com，而他回復了kevinf@flynnsarcade.com，我們將能夠跟蹤回復。 此外，如果您發電子郵件至flynn@flynnsarcade.com和CC alan@encom.com，而Alan又給您回信，它還會檢測到回復並結束活動。

## 如何跟蹤電子郵件附件 {#how-to-track-your-email-attachments}

Sales Connect提供對附件的跟蹤(.doc、.ppt和.pdf)，以便您可以查看其開啟/下載的時間，並查看您的收件人正在查看哪些頁面。 我們將允許您使用我們的可跟蹤附件功能 [Web應用](https://toutapp.com/login) 和Gmail(或Google應用)。

>[!NOTE]
>
>附件跟蹤僅適用於我們的團隊計畫（從g3啟動計劃開始）。

**如何發送第一個可跟蹤附件**

1. 撰寫電子郵件或編輯模板，然後按一下 **內容** 按鈕

1. 上傳附件併發送出去。 我們支援PDF、Word文檔和Powerpoint演示文稿。

1. 選擇 **添加到電子郵件**。

1. 按一下 **發送** 並點燃你的直播。 在收件人開啟並通過附件頁面時，您將看到他們。

>[!TIP]
>
>如果不想跟蹤附件，只需按一下「附加檔案」(Attach Files)，此附件將不會被跟蹤。

## 查看跟蹤的工作原理 {#how-view-tracking-works}

我們通過在您發送的電子郵件中放置不可見的影像來跟蹤開啟的電子郵件。

如果有人對您的電子郵件做出響應，但Sales Connect說未查看，則收件人很可能未在其電子郵件客戶端中啟用影像（即，按一下電子郵件中的「按一下這裡下載影像」消息）。

獲取電子郵件上更好跟蹤統計的一些提示：

* 在電子郵件中包括影像（如徽標），因此鼓勵收件人啟用影像以查看您的郵件。
* 在電子郵件中包括作為行動要求的連結。

## Test電子郵件未顯示為已查看 {#test-email-not-showed-as-viewed}

即使您將郵件發送到其他電子郵件地址，我們也不會記錄您查看您在即時訂閱源中發送給自己的任何電子郵件。 我們的跟蹤是基於設備的；只要您使用已登錄Sales Connect的電腦，我們就會過濾掉該活動。

原因何在？ Sales Connect是智慧的，如果我們的活動用戶每次查看他們發送的電子郵件時都在即時訂閱源活動中彈出自己的資訊，則永遠不會原諒我們。
