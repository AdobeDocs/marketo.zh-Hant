---
unique-page-id: 14352407
description: 傳送渠道概觀——行銷人員檔案——產品檔案
title: 傳送渠道概觀
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---


# 傳送渠道概述{#delivery-channel-overview}

Marketo Sales Connect為您提供多種發送電子郵件的選項。 本文將檢視您可運用的傳送管道、如何選取這些管道，以及何時選取一個管道。

## 建議：透過電子郵件連線的Gmail或Exchange {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect可透過我們的Email Connection服務簡化設定並增強傳遞能力。 Email Connection允許每個用戶將[Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)或[Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)帳戶連接到Sales Connect，以用作所有Sales Connect電子郵件的發送渠道。

使用Gmail或Exchange會比其他傳送通道選項有一些明顯的優勢：

* 這是一個久經考驗的傳送通道，其信譽卓著，有助於保持高傳送能力。
* IT團隊已配置和管理SPF和DKIM等驗證方法，因此不需要額外設定。
* 在指定的電子郵件網路內傳送電子郵件（即以Exchange使用者身分傳送電子郵件給透過Exchange接收電子郵件的公司）有助於進一步提高傳遞能力。

請務必注意，這些傳送管道有自己的傳送限制，由Microsoft和Google強制執行。 為了對抗此問題，我們運用節流機制來協助使用者維持這些限制。 在此瞭解有關[電子郵件調節的詳細資訊](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)。

>[!NOTE]
>
>依預設，O365外掛程式將一律使用您的交換傳送管道，而Gmail外掛程式則一律會利用您的Gmail傳送管道來傳送外掛程式的電子郵件。

**反彈追蹤**:MSC可偵測傳送至傳送者收件匣的彈回訊息，以偵測Exchange Online或Gmail使用者的彈回。這些彈回通知將統計至使用者的範本分析、促銷活動分析和即時動態消息通知。 Exchange On-Prem客戶不支援彈回數追蹤。

## 通過SMTP {#custom-delivery-channel-via-smtp}的自定義傳送通道

Sales Connect提供了連接第三方SMTP伺服器的附加選項，該伺服器將用作銷售團隊的首選傳送渠道。

對於以電子郵件數量為首的銷售團隊來說，使用第三方SMTP提供程式是一個絕佳的選項。 SMTP提供器（如Sendgrid和Sparkpost）經過優化，可滿足大量電子郵件傳送的需求，並可擴展以滿足那些希望部署大量電子郵件的用戶的需要。

此外，協力廠商SMTP提供者提供多種功能，以協助支援您團隊的傳送能力需求（例如電子郵件傳送報表和專屬IP位址），因此，對於想要在銷售電子郵件傳送管道中尋找更精細控制和可見度的人而言，這是絕佳的選擇。

## MSC伺服器（舊版）{#msc-servers-legacy}

MSC伺服器僅適用於某些舊版ToutApp客戶。 這些客戶將在其電子郵件設定中看到MSC伺服器。 所有非舊客戶將不把MSC視為一種選擇，應將其Gmail或Outlook帳戶連接至Sales Connect，以解鎖傳送渠道。

MSC伺服器不支援DKIM和SPF認證方法，這可以降低傳遞率。 因此，我們建議所有客戶都連接至Gmail或Outlook，以獲得最佳的傳遞能力。

## Marketo Servers {#marketo-servers}

Marketo電子郵件伺服器未與Sales Connect整合。 Marketo伺服器已最佳化，可大量傳送，讓伺服器可依行銷人員的需求進行擴充。 不過，Gmail和Exchange的1:1銷售通訊成功率較高，因此我們建議將這些伺服器用於您的銷售通訊。

>[!MORELIKETHIS]
>
>* [Gmail使用者的電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用戶的電子郵件連接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [設定自訂傳送渠道](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [電子郵件連接限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

