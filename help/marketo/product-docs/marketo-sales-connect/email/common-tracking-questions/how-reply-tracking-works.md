---
unique-page-id: 14352482
description: 回覆追蹤如何運作 — Marketo檔案 — 產品檔案
title: 回覆追蹤的運作方式
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# 回覆追蹤的運作方式 {#how-reply-tracking-works}

回覆追蹤的方式是查看您傳送之每封電子郵件中的訊息ID。 每封電子郵件都包含一個唯一的訊息ID，可讓我們進行一些最佳的回覆追蹤。

>[!PREREQUISITES]
>
>**與電子郵件伺服器的連接：** Sales Connect必須與您的收件箱連接，以便我們知道何時有新回復。 您需要有Sales Connect帳戶 [連接到Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). 如果您使用Outlook，我們需要與您的 [exchange伺服器](https://toutapp.com/next#settings/exchange_settings).

如果Sales Connect無法跟蹤您的潛在客戶對您電子郵件的回復，它將無法基於回複檢測停止促銷活動或記錄該回復到Salesforce。  什麼是電子郵件地址可以回覆？

這表示，如果您發電子郵件至flynn@flynnsarcade.com，而他以kevinf@flynnsarcade.com回應，我們便能追蹤回覆。 此外，如果您傳送電子郵件至flynn@flynnsarcade.com和CC alan@encom.com，而Alan回覆您，也會偵測回覆並結束促銷活動。
