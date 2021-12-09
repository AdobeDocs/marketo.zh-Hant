---
description: 傳遞管道概觀 — Marketo檔案 — 產品檔案
title: 傳遞通道概述
hide: true
hidefromtoc: true
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 0%

---

# 傳遞通道概述 {#delivery-channel-overview}

Marketo Sales可為您提供多種傳送電子郵件的選項。 本文將檢閱您可運用的傳送管道、如何選取管道，以及何時選取管道。

## 建議：透過Email Connection的Gmail或Exchange {#recommended-gmail-or-exchange-via-email-connection}

Marketo Sales可透過我們的電子郵件連線服務，簡化設定並增強傳遞能力。 電子郵件連線可讓每位使用者連線至 [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) 或 [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) 帳戶至Marketo銷售人員，以作為所有Marketo銷售電子郵件的傳送管道。

與其他傳送管道選項相比，使用Gmail或Exchange有一些明顯的優點：

* 這是經過驗證的傳遞渠道，其信譽卓著，有助於保持高傳遞能力。
* IT團隊已設定並管理SPF和DKIM等驗證方法，因此沒有其他設定。
* 在指定的電子郵件網路內傳送電子郵件（即以Exchange使用者身分傳送電子郵件給透過Exchange接收電子郵件的公司），有助於進一步提高傳遞能力。

請務必注意，這些傳送管道有各自的傳送限制，由Microsoft和Google強制執行。 為了克服這種情況，我們利用節流機制來幫助用戶保持在這些限制內。 深入了解 [此處提供電子郵件限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>依預設，O365外掛程式將一律使用您的交換傳送管道，而Gmail外掛程式將一律利用您的Gmail傳送管道，從外掛程式傳送電子郵件。

**跳出追蹤**:Marketo Sales可偵測傳送至寄件者收件匣的退信，以偵測Exchange Online或Gmail使用者的退信。 這些退信通知將統計至範本分析、行銷活動分析和使用者的即時摘要通知。 Exchange內部客戶不支援退信追蹤。

## 透過SMTP的自訂傳送通道 {#custom-delivery-channel-via-smtp}

Marketo Sales提供了連接第三方SMTP伺服器以用作銷售團隊首選的傳送渠道的其他選項。

對於以電子郵件數量為第一優先順序的銷售團隊來說，使用第三方SMTP提供者是絕佳的選擇。 SMTP提供程式（如Sendgrid和Sparkpost）經過優化，可滿足批量電子郵件傳送的需求，並可擴展以滿足那些希望部署大量電子郵件的提供者的需求。

此外，第三方SMTP提供者提供大量功能，以協助支援您團隊的傳遞需求（例如電子郵件傳送報告和專用的IP位址），因此對於那些想要獲得更精細控制並了解其銷售電子郵件傳送管道的人，這是絕佳的選擇。

## Marketo銷售伺服器（舊版） {#marketo-sales-servers-legacy}

Marketo銷售伺服器僅適用於某些舊版ToutApp客戶。 這些客戶會在其電子郵件設定中看到可用的Marketo銷售伺服器。 所有非舊版客戶將不視Marketo Sales為選項，應將其Gmail或Outlook帳戶連線至Marketo Sales，以解鎖傳遞管道。

Marketo銷售伺服器不支援DKIM和SPF驗證方法，這可能降低傳遞率。 因此，我們建議所有客戶連線至Gmail或Outlook，以獲得最佳的傳遞能力。

## MSC伺服器（舊版） {#msc-servers-legacy}

MSC伺服器僅適用於某些舊版ToutApp客戶。 這些客戶將在其電子郵件設定中看到MSC伺服器可用。 所有非舊版客戶將不會將MSC視為選項，應將其Gmail或Outlook帳戶連接至Sales Connect，以解鎖傳送通道。

MSC伺服器不支援DKIM和SPF驗證方法，這會降低傳遞率。 因此，我們建議所有客戶連線至Gmail或Outlook，以獲得最佳的傳遞能力。

## Marketo伺服器 {#marketo-servers}

Marketo電子郵件伺服器未與Marketo銷售整合。 Marketo伺服器已針對大量傳送進行最佳化，以便根據行銷人員的需求進行擴充。 不過，Gmail和Exchange在1:1銷售通訊方面的成功率較高，因此我們建議將這些伺服器用於您的銷售通訊。

>[!MORELIKETHIS]
>
>* [Gmail使用者的電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用戶的電子郵件連接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [設定自訂傳送通道](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [電子郵件連線限制](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

