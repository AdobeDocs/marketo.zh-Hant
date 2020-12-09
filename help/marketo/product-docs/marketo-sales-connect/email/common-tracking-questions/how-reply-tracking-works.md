---
unique-page-id: 14352482
description: 回覆追蹤的運作方式——行銷檔案——產品檔案
title: 回覆追蹤的運作方式
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# 回覆追蹤的運作方式 {#how-reply-tracking-works}

回覆追蹤是透過查看您傳送之每封電子郵件中的訊息ID來完成。 每封電子郵件都包含一個唯一的訊息ID，可讓我們進行一些最佳的回覆追蹤。

>[!PREREQUISITES]
>
>**與電子郵件伺服器的連接：** Sales Connect必須與您的收件箱連接，以便我們知道何時收到新的回復。 您需要將Sales Connect帳戶連 [接到Gmail](http://docs.marketo.com/x/kYMOAQ)。 如果您使用Outlook，我們需要與您的Exchange伺服器 [整合](http://toutapp.com/next#settings/exchange_settings)。

如果Sales Connect無法追蹤潛在客戶對您電子郵件的回覆，將無法根據回覆偵測或記錄回覆至Salesforce的促銷活動。  我們指的是，任何電子郵件地址都能回覆？

這表示如果您以電子郵 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) 件傳送他回覆 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad)，我們就可以追蹤回覆。 此外，如果您以電子郵 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) 件和CC寄 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153)回給您，Alan也會回覆您，它會偵測回覆並結束促銷活動。
