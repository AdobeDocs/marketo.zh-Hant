---
unique-page-id: 14352407
description: 傳遞管道概觀 — Marketo檔案 — 產品檔案
title: 傳遞管道總覽
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# 傳遞管道總覽 {#delivery-channel-overview}

Marketo Sales Connect提供您多種傳送電子郵件的選項。 本文將檢閱您可以運用的傳送管道、如何選取管道，以及何時應選取管道而不應選取管道。

## 建議：透過電子郵件連線的Gmail或Exchange {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect可簡化設定，並透過我們的電子郵件連線服務增強傳遞能力。 電子郵件連線可讓每位使用者連線至他們的[Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)或[Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)帳戶至Sales Connect，以作為所有Sales Connect電子郵件的傳遞選擇管道。

與其他傳遞管道選項相比，使用Gmail或Exchange具有一些明顯的優勢：

* 這是一個備受肯定的傳送管道，並擁有良好的聲譽，有助於保持高傳送能力。
* SPF和DKIM等驗證方法已由IT團隊設定和管理，因此無需額外設定。
* 在指定的電子郵件網路內傳送電子郵件（即以Exchange使用者的身分傳送電子郵件給透過Exchange接收電子郵件的公司）可進一步提升傳遞能力。

請務必注意，這些傳送管道有其本身的傳送限制，而這些限制是由Microsoft和Google強制執行。 為克服此情況，我們採用節流機制來協助使用者符合這些限制。 在此進一步瞭解[電子郵件節流](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)。

>[!NOTE]
>
>根據預設，O365外掛程式一律會使用您的Exchange傳遞管道，而Gmail外掛程式則一律會使用您的Gmail傳遞管道，傳遞外掛程式中的電子郵件。

**跳出追蹤**： MSC可偵測傳送到寄件者收件匣的跳出訊息，以偵測Exchange Online或Gmail使用者的跳出。 這些跳出通知將彙總到使用者的範本分析、行銷活動分析和即時摘要通知中。 Exchange內部部署客戶不支援跳出追蹤。

## 透過SMTP的自訂傳遞頻道 {#custom-delivery-channel-via-smtp}

Sales Connect提供額外選項，可連線第三方SMTP伺服器，以作為銷售團隊偏好的傳遞管道。

對於電子郵件數量是第一優先順序的銷售團隊而言，使用協力廠商SMTP提供者是一個很好的選擇。 Sendgrid和Sparkpost等SMTP提供者已最佳化，以符合大量電子郵件傳送的需求，且可擴充以滿足希望部署大量電子郵件的需求。

此外，第三方SMTP提供者提供大量功能，可協助支援您團隊的傳遞能力需求（例如電子郵件傳遞報告和專用IP位址），因此對於需要更精細的控制以及銷售電子郵件傳遞通道可見度的使用者而言，這是一個絕佳選項。

## MSC伺服器（舊版） {#msc-servers-legacy}

MSC伺服器僅供某些舊版ToutApp客戶使用。 這些客戶會在電子郵件設定中看到MSC伺服器。 所有非舊版客戶不會看到MSC作為選項，而應將其Gmail或Outlook帳戶連線至Sales Connect以解除鎖定傳遞管道。

MSC伺服器不支援DKIM和SPF驗證方法，這會降低傳遞率。 因此，我們建議所有客戶連線至Gmail或Outlook，以獲得最佳傳遞能力。

## Marketo伺服器 {#marketo-servers}

Marketo電子郵件伺服器未與Sales Connect整合。 Marketo伺服器已針對大量傳送進行最佳化，可因應行銷人員的需求進行擴充。 不過，Gmail和Exchange在1:1銷售通訊的成功率較高，因此我們建議使用這些伺服器進行銷售通訊。

>[!MORELIKETHIS]
>
>* Gmail使用者的[電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [電子郵件連線給Outlook使用者](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [設定自訂傳遞通道](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [電子郵件連線節流](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
