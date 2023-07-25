---
description: 電子郵件追蹤概述 — Marketo檔案 — 產品檔案
title: 電子郵件追蹤概觀
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 電子郵件追蹤概觀 {#email-tracking-overview}

## 回覆追蹤的運作方式 {#how-reply-tracking-works}

「回覆追蹤」是透過檢視您傳送之每封電子郵件中的訊息ID來完成。 每封電子郵件都包含唯一的訊息ID，讓我們有一些最佳的回覆追蹤功能。

>[!PREREQUISITES]
>
>與電子郵件伺服器的連線： Sales Connect必須與您的收件匣連線，以便我們知道何時收到新回覆。 您必須將您的Sales Connect帳戶連線至Gmail。 如果您使用Outlook，我們需要與您的Exchange伺服器整合。

如果Sales Connect無法追蹤潛在客戶對您的電子郵件的回覆，將無法根據回覆偵測停止行銷活動或將回覆記錄到Salesforce。 我們所說的電子郵件地址可以回覆是什麼意思？

這表示如果您傳送電子郵件給flynn@flynnsarcade.com，而他使用kevinf@flynnsarcade.com回應，我們就能追蹤回應。 此外，如果您以電子郵件傳送flynn@flynnsarcade.com和CC alan@encom.com，而Alan回寫您，它也會偵測回覆並結束行銷活動。

## 如何追蹤您的電子郵件附件 {#how-to-track-your-email-attachments}

Sales Connect提供附件(.doc、.ppt、.pdf)上的追蹤功能，讓您檢視附件何時開啟/下載，以及收件者瀏覽的頁面。 我們將允許您同時使用以下兩個來源的可追蹤附件功能： [網頁應用程式](https://toutapp.com/login) 和Gmail (或Google應用程式)。

>[!NOTE]
>
>附件追蹤僅適用於我們的團隊計畫（從我們的g3startup計劃開始）。

**如何傳送您的第一個可追蹤附件**

1. 撰寫電子郵件或編輯範本，然後按一下 **內容** 按鈕。

1. 上傳附件並將其寄出。 我們支援PDF、Word檔案和Powerpoint簡報。

1. 選取 **新增至電子郵件**.

1. 按一下 **傳送** 並引發您的即時摘要。 您會在收件者開啟並瀏覽附件時看到收件者。

>[!TIP]
>
>如果您不想追蹤附件，只要按一下[附加檔案]，就不會追蹤此附件。

## 檢視追蹤的運作方式 {#how-view-tracking-works}

我們會在您傳送的電子郵件內放置不可見的影像，以追蹤電子郵件開啟次數。

如果有人回覆您的電子郵件，但Sales Connect指出未檢視該電子郵件，則收件者未在其電子郵件使用者端內啟用影像的機率為何（亦即，按一下電子郵件中的「按一下這裡以下載影像」訊息）。

在電子郵件上取得更佳追蹤統計資料的一些秘訣：

* 在電子郵件中加入影像（例如標誌），鼓勵收件者啟用影像功能來檢視您的訊息。
* 在電子郵件中加入連結作為行動號召。

## 測試電子郵件未顯示為已檢視 {#test-email-not-showed-as-viewed}

即使您將訊息傳送至其他電子郵件地址，我們也不會記錄您在「即時摘要」中檢視您傳送給自己的任何電子郵件。 我們的追蹤是以裝置為基礎；只要您使用已登入Sales Connect的電腦，我們就會篩選掉該活動。

原因何在？ Sales Connect很聰明，而且我們的活躍使用者絕不會原諒我們，只要他們每次檢視傳送的電子郵件時，就會在即時摘要活動中彈出他們自己的資訊。
