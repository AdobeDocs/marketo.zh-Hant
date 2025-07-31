---
description: 電子郵件連線節流 — Marketo檔案 — 產品檔案
title: 電子郵件連線節流
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
feature: Sales Insight Actions
source-git-commit: b4e5d17aa882a89b01f77f875312b0d71aa754f3
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 電子郵件連線節流 {#email-connection-throttling}

整合要透過[!DNL Sales Connect]或Gmail電子郵件提供者傳送的[!DNL Exchange]帳戶，提供簡化的設定，並最佳化1:1銷售通訊的電子郵件傳遞能力。 不過，為了維持系統健康且帳戶安全，Gmail和[!DNL Exchange]會強制執行電子郵件傳送限制。 這些限制可由提供者自行決定增加或減少。

## 概觀 {#overview}

電子郵件連線節流可讓Sales Connect管理員設定使用Gmail或Exchange作為傳遞管道時電子郵件的傳送速率，如此一來，將電子郵件傳送給傳遞管道提供者的速率，便不會超過強制的限制。

當限制一律超過時，這有時可視為來自傳送通道提供者的可疑行為，導致電子郵件失敗，有時甚至會停用帳戶。

## 注意事項 {#things-to-note}

* 當使用者連線到Gmail或[!DNL Exchange]時自動啟用
* 如果您想要從建議中增加或減少設定以符合您的需求，則可自訂
* 僅節流透過Gmail或[!DNL Exchange]傳送的電子郵件，不會節流自訂傳遞通道
* 電子郵件連線節流會個別將每位使用者的電子郵件加入佇列，因為每位使用者有其自己與電子郵件提供者的連線

## 正在設定電子郵件連線節流設定 {#configuring}

1. 按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/email-connection-throttling-1.png)

1. 在[!UICONTROL Admin Settings]底下，按一下&#x200B;**[!UICONTROL General]**。

   ![](assets/email-connection-throttling-2.png)

1. 在右側的電子郵件連線節流卡中，按一下&#x200B;**[!UICONTROL Enable Email Throttling]**&#x200B;滑桿。

   ![](assets/email-connection-throttling-3.png)

1. 在右側的電子郵件連線節流卡中，輸入傳送給電子郵件通道提供者所需的電子郵件批次大小。

   ![](assets/email-connection-throttling-4.png)

1. 設定每個批次傳送前的等待時間。 在此範例中，我們每45秒選擇25封電子郵件。

   ![](assets/email-connection-throttling-5.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/email-connection-throttling-6.png)

儲存變更後，所有使用者都會將電子郵件批次傳送至其連線的Gmail或[!DNL Exchange]帳戶以進行傳遞。

## 電子郵件提供者限制 {#email-provider-limits}

### [!DNL Outlook 365] {#outlook}

商業/企業

* 每天10,000
* 每分鐘30次
* 每封電子郵件500位收件者

如需詳細資訊[，請參閱此處](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)。

### Gmail {#gmail}

* 每天2000個（試用和標幟帳戶為500個）
* 每秒2封電子郵件（API限制）
* 每則訊息2,000位收件者（外部收件者最多500位）

如需詳細資訊[，請參閱此處](https://support.google.com/a/answer/166852?hl=en)。

### [!DNL Microsoft Exchange Server (2010, 2013)] {#microsoft-exchange}

限制由組織的IT部門設定，因為伺服器由組織託管。 如有其他資訊，請聯絡網路或系統管理員。

>[!MORELIKETHIS]
>
>* [傳遞管道總覽](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* Gmail使用者的[電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [電子郵件連線給Outlook使用者](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
