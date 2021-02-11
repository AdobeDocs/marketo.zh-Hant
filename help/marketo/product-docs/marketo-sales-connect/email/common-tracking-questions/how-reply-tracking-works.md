---
unique-page-id: 14352482
description: 回覆追蹤的運作方式——行銷檔案——產品檔案
title: 回覆追蹤的運作方式
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 回覆追蹤的運作方式{#how-reply-tracking-works}

回覆追蹤是透過查看您傳送之每封電子郵件中的訊息ID來完成。 每封電子郵件都包含一個唯一的訊息ID，可讓我們進行一些最佳的回覆追蹤。

>[!PREREQUISITES]
>
>**與電子郵件伺服器的連** 接： Sales Connect必須與您的收件箱連接，以便我們知道何時收到新的回復。您需要將Sales Connect帳戶[連接到Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-tab-for-gmail-users.md)。 如果您使用Outlook，我們需要與[exchange伺服器](https://toutapp.com/next#settings/exchange_settings)整合。

如果Sales Connect無法追蹤潛在客戶對您電子郵件的回覆，將無法根據回覆偵測或記錄回覆至Salesforce的促銷活動。  我們指的是，任何電子郵件地址都能回覆？

這表示，如果您以電子郵件寄送flynn@flynnsarcade.com，而他以kevinf@flynnsarcade.com回覆，我們就可以追蹤回覆。 此外，如果您以電子郵件寄送flynn@flynnsarcade.com和CC alan@encom.com，而Alan又將您回信，它也會偵測回覆並結束促銷活動。
