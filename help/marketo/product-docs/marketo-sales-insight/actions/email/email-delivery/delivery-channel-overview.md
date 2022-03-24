---
description: 交付渠道概述 — Marketo文檔 — 產品文檔
title: 交付渠道概述
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 交付渠道概述 {#delivery-channel-overview}

Marketo銷售部為您提供多種電子郵件發送選項。 本文將回顧您可以利用的交付渠道、如何選擇這些渠道以及何時選擇它們。

## 建議：通過電子郵件連接Gmail或Exchange {#recommended-gmail-or-exchange-via-email-connection}

Marketo銷售人員通過我們的電子郵件連接服務實現了簡化的設定和增強的交付能力。 電子郵件連接允許每個用戶連接到其 [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) 或 [交換](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) 客戶到Marketo銷售部，作為所有Marketo銷售電子郵件的交付渠道。

利用Gmail或Exchange與其他遞送渠道選項相比，具有一些獨特的優勢：

* 這是一個久經考驗的交付渠道，擁有良好的聲譽，有助於保持高交付能力。
* IT團隊已配置和管理SPF和DKIM等身份驗證方法，因此沒有其他設定。
* 在給定電子郵件網路內發送電子郵件（即以Exchange用戶身份向通過Exchange接收電子郵件的公司發送電子郵件）有助於進一步提高可交付性。

必須注意的是，這些傳送渠道有自己的傳送限制，由Microsoft和Google執行。 為了克服這一問題，我們使用限制機制來幫助用戶保持在這些限制範圍內。 瞭解有關 [此處的電子郵件限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)。

>[!NOTE]
>
>預設情況下，O365插件將始終使用您的交換傳遞渠道，而Gmail插件將始終利用您的Gmail傳遞渠道來傳遞插件中的電子郵件。

**彈跳跟蹤**:Marketo銷售人員可以通過檢測發送到發件人收件箱的彈回郵件來檢測Exchange Online或Gmail用戶的回報。 這些退貨通知將匯總到用戶的模板分析、市場活動分析和即時訂閱源通知中。 Exchange On-Prem客戶不支援彈跳跟蹤。

## 通過SMTP的自定義傳遞通道 {#custom-delivery-channel-via-smtp}

Marketo銷售人員提供了連接第三方SMTP伺服器以用作銷售團隊首選的交付渠道的附加選項。

對於以電子郵件量為首要優先順序的銷售團隊而言，利用第三方SMTP提供商是一個絕佳選擇。 SMTP提供程式（如Sendgrid和Sparkpost）已經過優化，可滿足批量電子郵件傳遞的需要，並可以擴展以滿足那些希望部署大量電子郵件的需要。

此外，第三方SMTP提供商提供了大量功能來幫助支援您團隊的可交付性需求（如電子郵件交付報告和專用IP地址），因此對於那些希望對其銷售電子郵件交付渠道進行更細的控制和查看的人來說，這是一個絕佳的選擇。

## Marketo銷售伺服器（舊版） {#marketo-sales-servers-legacy}

Marketo銷售伺服器僅適用於一些舊式ToutApp客戶。 這些客戶將在其電子郵件設定中看到Marketo銷售伺服器。 所有非傳統客戶都不會將Marketo銷售視為一種選擇，應將他們的Gmail或Outlook帳戶連接到Marketo銷售，以解鎖交付渠道。

Marketo銷售伺服器不支援DKIM和SPF身份驗證方法，這會降低傳輸率。 因此，我們建議所有客戶都連接到Gmail或Outlook，以獲得最佳的可交付性。

## MSC伺服器（舊版） {#msc-servers-legacy}

MSC伺服器僅適用於某些舊式ToutApp客戶。 這些客戶將在電子郵件設定中看到MSC伺服器可用。 所有非傳統客戶將不會將MSC視為一個選項，應將其Gmail或Outlook帳戶連接到Sales Connect以解鎖傳遞渠道。

MSC伺服器不支援DKIM和SPF認證方法，這會降低傳輸率。 因此，我們建議所有客戶都連接到Gmail或Outlook，以獲得最佳的可交付性。

## Marketo伺服器 {#marketo-servers}

Marketo電子郵件伺服器不與Marketo銷售部整合。 Marketo伺服器經過優化，可以批量交付，以滿足營銷人員的需求。 但是，Gmail和Exchange在1:1銷售通信中的成功率更高，因此我們建議將這些伺服器用於您的銷售通信。

>[!MORELIKETHIS]
>
>* [Gmail用戶的電子郵件連接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用戶的電子郵件連接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [設定自定義交付渠道](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [電子郵件連接限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

