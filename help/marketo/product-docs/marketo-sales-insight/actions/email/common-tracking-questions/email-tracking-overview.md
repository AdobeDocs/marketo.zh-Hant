---
description: Email Tracking Overview - Marketo Docs - Product Documentation
title: 電子郵件追蹤概述
hide: true
hidefromtoc: true
source-git-commit: 8789ed464f532bbe76c2cb456374d9c0f505ece0
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# 電子郵件追蹤概述 {#email-tracking-overview}

## How Reply Tracking Works {#how-reply-tracking-works}

Reply Tracking is done by looking at a message ID that’s in every email you send. 每封電子郵件都包含一個唯一的訊息ID，可讓我們進行一些最佳的回覆追蹤。

>[!PREREQUISITES]
>
>與電子郵件伺服器的連接：Sales Connect必須與您的收件箱連接，以便我們知道何時有新回復。 您的Sales Connect帳戶必須連接到Gmail。 If you’re using Outlook, we’ll need to integrate with your exchange server.

如果Sales Connect無法跟蹤您的潛在客戶對您電子郵件的回復，它將無法基於回複檢測停止促銷活動或記錄該回復到Salesforce。 什麼是電子郵件地址可以回覆？

這表示，如果您發電子郵件至flynn@flynnsarcade.com，而他以kevinf@flynnsarcade.com回應，我們便能追蹤回覆。 此外，如果您傳送電子郵件至flynn@flynnsarcade.com和CC alan@encom.com，而Alan回覆您，也會偵測回覆並結束促銷活動。

## 回覆追蹤的運作方式 {#how-reply-tracking-works}

文字

## 如何追蹤電子郵件附件 {#how-to-track-your-email-attachments}

