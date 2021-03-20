---
description: 電子郵件連線限制——行銷人員檔案——產品檔案
title: 電子郵件連接限制
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---


# 電子郵件連接調節{#email-connection-throttling}

整合您的Sales Connect帳戶，以透過Exchange或Gmail電子郵件提供者傳送，提供簡化的設定，並最佳化1:1銷售通訊的電子郵件傳送能力。 不過，為了保持系統健康和安全，Gmail和Exchange強制實施電子郵件發送限制。 供應商可自行決定增加或減少這些限制。

## 電子郵件連接調節（測試版）{#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>此功能目前在測試版中。 若要加入此測試版，請連絡您的客戶成功經理。

Email Connection Throttling允許Sales Connect管理員在使用Gmail或Exchange作為您的傳送渠道時，設定電子郵件的傳送速率，以便將電子郵件傳送給傳送渠道供應商的速率不會超過強制限制。

當持續超過限制時，有時會被視為來自傳送渠道供應商的可疑行為，導致電子郵件失敗，有時甚至會停用帳戶。

**附註／重點說明**

* 使用者連線至Gmail或Exchange時自動啟用
* 如果您想要根據需求增加或減少建議的設定，可自訂
* 只限制透過Gmail或Exchange傳送的電子郵件，不會限制自訂傳送管道
* 「電子郵件連線」調節功能會將每位個別使用者的電子郵件分別排入佇列，因為每位使用者都與其電子郵件供應商有各自的連線

**配置電子郵件連接調節設定**

1. 按一下齒輪表徵圖並選擇「**設定**」。

   ![](assets/email-connection-throttling-1.png)

1. 按一下&#x200B;**常規**。

   ![](assets/email-connection-throttling-2.png)

1. 在「電子郵件連線限制」卡中，輸入所要的電子郵件批次大小，這些電子郵件將傳送給電子郵件通路供應商。

   ![](assets/email-connection-throttling-3.png)

1. 設定每個批發送前要等待的時間。 在此範例中，我們每45秒選擇25封電子郵件。

   ![](assets/email-connection-throttling-4.png)

1. 按一下&#x200B;**保存**。

   ![](assets/email-connection-throttling-5.png)

在保存這些更改後，所有用戶將分批將電子郵件發送到其連接的Gmail或Exchange帳戶，以便發送。

## 電子郵件提供者限制{#email-provider-limits}

**Outlook 365**

企業／企業

* 每天10,000
* 每分鐘30人
* 每封電子郵件有500位收件者

如需詳細資訊[，請參閱](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)。

**Gmail**

* 每天2000人（500人適用於試用版和標幟帳戶）
* 每秒2封電子郵件（API限制）
* 每封訊息2,000位收件者（外部收件者最多500位）

如需詳細資訊[，請參閱](https://support.google.com/a/answer/166852?hl=en)。

**Microsoft Exchange Server(2010、2013)**

限制由組織的IT部門設定，因為伺服器由組織托管。 如需詳細資訊，請洽詢網路或系統管理員。

>[!MORELIKETHIS]
>
>* [傳送渠道概觀](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Gmail使用者的電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用戶的電子郵件連接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

