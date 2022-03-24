---
description: 電子郵件連接限制 — Marketo文檔 — 產品文檔
title: 電子郵件連接限制
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 電子郵件連接限制 {#email-connection-throttling}

將您的Sales Connect帳戶整合到Exchange或Gmail電子郵件提供商中，可簡化設定並優化1:1銷售通信的電子郵件傳送能力。 然而，為了保持系統健康和賬戶安全，Gmail和Exchange強制實施電子郵件發送限制。 供應商可酌情決定增加或減少該等限額。

## 電子郵件連接限制(Beta) {#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>此功能當前在Beta版中。 要加入此試用版，請與您的客戶成功經理聯繫。

電子郵件連接限制允許銷售連接管理員在將Gmail或Exchange用作您的傳遞渠道時配置電子郵件的發送速率，以便將電子郵件移交給傳遞渠道提供商的速率不超過強制限制。

當持續超過限制時，有時會被視為來自傳遞渠道提供商的可疑行為，導致電子郵件失敗，有時甚至會禁用帳戶。

**注釋/亮點**

* 用戶連接到Gmail或Exchange後自動啟用
* 如果希望根據建議增加或減少設定以滿足您的需要，可以自定義
* 只限制通過Gmail或Exchange發送的電子郵件，不限制自定義傳遞渠道
* 「電子郵件連接」限制將分別將每個用戶的電子郵件排隊，因為每個用戶都與其電子郵件提供商有各自的連接

**配置電子郵件連接限制設定**

1. 按一下齒輪表徵圖並選擇 **設定**。

   ![](assets/email-connection-throttling-1.png)

1. 在「Admin Settings（管理設定）」下，按一下 **常規**。

   ![](assets/email-connection-throttling-2.png)

1. 在右側的「Email Connection Throttling（電子郵件連接限制）」卡中，按一下 **啟用電子郵件限制** 按鈕。

   ![](assets/email-connection-throttling-3.png)

1. 在右側的「電子郵件連接限制」卡中，輸入要發送到電子郵件渠道提供商的電子郵件批量大小。

   ![](assets/email-connection-throttling-4.png)

1. 設定發送每個批之前等待的時間。 在此示例中，我們每45秒選擇25封電子郵件。

   ![](assets/email-connection-throttling-5.png)

1. 按一下 **保存**。

   ![](assets/email-connection-throttling-6.png)

保存更改後，所有用戶都將其電子郵件批量發送到其連接的Gmail或Exchange帳戶以進行傳遞。

## 電子郵件提供程式限制 {#email-provider-limits}

**展望365**

企業/企業

* 每天10,000
* 每分鐘30人
* 每封電子郵件500個收件人

詳細資訊 [可在此處找到](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)。

**Gmail**

* 每天2000人（500人用於試用和標籤帳戶）
* 每秒2封電子郵件（API限制）
* 每封郵件2,000個收件人（外部收件人最多500個）

詳細資訊 [可在此處找到](https://support.google.com/a/answer/166852?hl=en)。

**MicrosoftExchange Server(2010、2013)**

限制由組織的IT部門設定，因為伺服器由組織托管。 如需其他資訊，請聯繫網路或系統管理員。

>[!MORELIKETHIS]
>
>* [交付渠道概述](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Gmail用戶的電子郵件連接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用戶的電子郵件連接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

