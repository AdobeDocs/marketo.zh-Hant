---
unique-page-id: 14352482
description: 回覆追蹤的運作方式 — Marketo檔案 — 產品檔案
title: 回覆追蹤的運作方式
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# 回覆追蹤的運作方式 {#how-reply-tracking-works}

「回覆追蹤」是透過檢視您傳送之每封電子郵件中的訊息ID來完成。 每封電子郵件都包含唯一的訊息ID，讓我們擁有一些最佳的回覆追蹤功能。

>[!PREREQUISITES]
>
>**與電子郵件伺服器的連線：** [!DNL Sales Connect]必須與您的收件匣連線，以便我們得知何時收到新的回覆。 您必須將您的[!DNL Sales Connect]帳戶[連線至Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)。 如果您使用[!DNL Outlook]，我們需要與您的[Exchange伺服器](https://toutapp.com/next#settings/exchange_settings)整合。

如果[!DNL Sales Connect]無法追蹤潛在客戶對您的電子郵件的回覆，將無法根據回覆偵測停止行銷活動或將回覆記錄到[!DNL Salesforce]。  什麼是任何電子郵件地址可以回覆？

這表示如果您傳送電子郵件給flynn@flynnsarcade.com，而他使用kevinf@flynnsarcade.com回應，我們就能追蹤回應。 此外，如果您以電子郵件傳送flynn@flynnsarcade.com和CC alan@encom.com ，而Alan將您回寫，它也會偵測回覆並結束行銷活動。
