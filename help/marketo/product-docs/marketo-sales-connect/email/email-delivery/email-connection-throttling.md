---
description: 電子郵件連線限制 — Marketo檔案 — 產品檔案
title: 電子郵件連線限制
exl-id: 093f5459-1bbb-45dd-8590-71ea4e1168d4
source-git-commit: ad7b222c2da937474565729a09a559fbcd722280
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 電子郵件連線限制 {#email-connection-throttling}

整合您的Sales Connect帳戶，以透過Exchange或Gmail電子郵件提供者傳送，提供簡化的設定，並最佳化電子郵件傳遞，以提供1:1的銷售通訊。 不過，為了確保系統健康且帳戶安全，Gmail和Exchange強制實施電子郵件傳送限制。 這些限制可由提供者自行決定增加或減少。

## 總覽 {#overview}

「電子郵件連線限制」可讓Sales Connect管理員在使用Gmail或Exchange作為您的傳送管道時，設定電子郵件的傳送率，如此一來，將電子郵件傳遞至傳送管道提供者的速度，就不會超過強制的限制。

當持續超過限制時，有時會被視為來自傳送管道提供者的可疑行為，導致電子郵件失敗，有時甚至帳戶也會停用。

**附註/重點**

* 使用者連線至Gmail或Exchange時自動啟用
* 如果您想要根據自己的需求增加或減少建議的設定，可加以自訂
* 僅限制通過Gmail或Exchange發送的電子郵件，不限制自訂傳送通道
* 「電子郵件連線」節流會讓每個個別使用者分別進入佇列，因為每個使用者都與其電子郵件提供者有各自的連線

**配置電子郵件連接限制設定**

1. 按一下齒輪圖示並選取 **設定**.

   ![](assets/email-connection-throttling-1.png)

1. 按一下 **一般**.

   ![](assets/email-connection-throttling-2.png)

1. 在「電子郵件連線限制」卡中，輸入要傳送給電子郵件通道提供者之電子郵件的所需批次大小。

   ![](assets/email-connection-throttling-3.png)

1. 設定每個批發送前的等待時間。 在此範例中，我們每45秒會選擇25封電子郵件。

   ![](assets/email-connection-throttling-4.png)

1. 按一下 **儲存**.

   ![](assets/email-connection-throttling-5.png)

儲存變更後，所有使用者都會將電子郵件分批傳送至其連線的Gmail或Exchange帳戶，以供傳送。

## 電子郵件提供者限制 {#email-provider-limits}

**Outlook 365**

企業/企業

* 每天10,000
* 每分鐘30
* 每封電子郵件有500個收件者

更多資訊 [可在此處找到](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 每天2000人（500人用於試用帳戶和已標籤帳戶）
* 每秒2封電子郵件（API限制）
* 每封訊息2,000個收件者（外部收件者最多500個）

更多資訊 [可在此處找到](https://support.google.com/a/answer/166852?hl=en).

**Microsoft Exchange Server(2010、2013)**

由組織的IT部門設定限制，因為伺服器由組織托管。 如需詳細資訊，請聯絡網路或系統管理員。

>[!MORELIKETHIS]
>
>* [傳遞通道概述](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Gmail使用者的電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用戶的電子郵件連接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

