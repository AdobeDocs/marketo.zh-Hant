---
description: 電子郵件追蹤概述 — Marketo檔案 — 產品檔案
title: 電子郵件追蹤概述
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 電子郵件追蹤概述 {#email-tracking-overview}

## 回覆追蹤的運作方式 {#how-reply-tracking-works}

回覆追蹤的方式是查看您傳送之每封電子郵件中的訊息ID。 每封電子郵件都包含一個唯一的訊息ID，可讓我們進行一些最佳的回覆追蹤。

>[!PREREQUISITES]
>
>與電子郵件伺服器的連接：Sales Connect必須與您的收件箱連接，以便我們知道何時有新回復。 您的Sales Connect帳戶必須連接到Gmail。 如果您使用Outlook，我們需要與您的exchange伺服器整合。

如果Sales Connect無法跟蹤您的潛在客戶對您電子郵件的回復，它將無法基於回複檢測停止促銷活動或記錄該回復到Salesforce。 什麼是電子郵件地址可以回覆？

這表示，如果您發電子郵件至flynn@flynnsarcade.com，而他以kevinf@flynnsarcade.com回應，我們便能追蹤回覆。 此外，如果您傳送電子郵件至flynn@flynnsarcade.com和CC alan@encom.com，而Alan回覆您，也會偵測回覆並結束促銷活動。

## 如何追蹤電子郵件附件 {#how-to-track-your-email-attachments}

Sales Connect優惠方案會追蹤您的附件(.doc、.ppt、.pdf)，讓您查看其開啟/下載的時間，以及查看收件者正在查看的頁面。 我們將允許您使用來自 [網頁應用程式](https://toutapp.com/login) 和Gmail(或Google應用程式)。

>[!NOTE]
>
>附件追蹤僅適用於我們的團隊計畫（從g3startup計劃開始）。

**如何傳送您的第一個可追蹤附件**

1. 撰寫電子郵件或編輯範本，然後按一下 **內容** 按鈕。

1. 上傳附件並送出。 我們支援PDF、Word文檔和Powerpoint演示文稿。

1. 選擇 **新增至電子郵件**.

1. 按一下 **傳送** 並啟動即時摘要。 您會在收件者開啟並翻閱附件時看到他們。

>[!TIP]
>
>如果您不想追蹤附件，只需按一下「附加檔案」，就不會追蹤此附件。

## 檢視追蹤如何運作 {#how-view-tracking-works}

我們會在您傳送的電子郵件中放置隱藏的影像，以追蹤電子郵件開啟次數。

如果某人回覆了您的電子郵件，但Sales Connect表示未檢視，則收件者在其電子郵件用戶端內未啟用影像的可能性為（亦即，按一下電子郵件中的「按一下這裡下載影像」訊息）。

一些在電子郵件上取得更佳追蹤統計資料的秘訣：

* 在電子郵件中加入影像（如標誌），以鼓勵收件者讓影像看見您的訊息。
* 在電子郵件中加入連結，作為動作呼叫。

## 測試電子郵件未顯示為已檢視 {#test-email-not-showed-as-viewed}

即使您將訊息傳送至其他電子郵件地址，我們也不會在即時資訊源中記錄您檢視任何您傳送給自己的電子郵件。 我們的追蹤是以裝置為基礎；只要您使用的電腦已登錄到Sales Connect，我們就會過濾該活動。

原因是什麼？ Sales Connect是智慧型的，我們的活躍使用者每次查看他們寄送的電子郵件時，如果在即時摘要活動中出現其自己的資訊，就不會原諒我們。
