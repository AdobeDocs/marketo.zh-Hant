---
description: 電子郵件連線節流 — Marketo檔案 — 產品檔案
title: 電子郵件連線節流
exl-id: 093f5459-1bbb-45dd-8590-71ea4e1168d4
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 2%

---

# 電子郵件連線節流 {#email-connection-throttling}

整合要透過[!DNL Sales Connect]或Gmail電子郵件提供者傳送的[!DNL Exchange]帳戶，提供簡化的設定，並最佳化1:1銷售通訊的電子郵件傳遞能力。 不過，為了維持系統健康且帳戶安全，Gmail和Exchange會強制實施電子郵件傳送限制。 這些限制可由提供者自行決定增加或減少。

## 概觀 {#overview}

電子郵件連線節流可讓[!DNL Sales Connect]管理員在使用Gmail或[!DNL Exchange]作為傳遞通道時，設定電子郵件的傳送速率，如此一來，將電子郵件傳送給傳遞通道提供者的速率就不會超過強制的限制。

當限制一律超過時，這有時可視為來自傳送通道提供者的可疑行為，導致電子郵件失敗，有時甚至會停用帳戶。

**附註/重點提示**

* 使用者連線至Gmail或[!DNL Exchange]後自動啟用
* 如果您想要從建議中增加或減少設定以符合您的需求，則可自訂
* 僅節流透過Gmail或[!DNL Exchange]傳送的電子郵件，不會節流自訂傳遞通道
* 電子郵件連線節流會個別將每位使用者的電子郵件加入佇列，因為每位使用者有其自己與電子郵件提供者的連線

**正在設定您的電子郵件連線節流設定**

1. 按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/email-connection-throttling-1.png)

1. 按一下「**[!UICONTROL General]**」。

   ![](assets/email-connection-throttling-2.png)

1. 在「電子郵件連線節流」卡片中，輸入要傳送給電子郵件通道提供者的電子郵件批次大小。

   ![](assets/email-connection-throttling-3.png)

1. 設定每個批次傳送前的等待時間。 在此範例中，我們每45秒選擇25封電子郵件。

   ![](assets/email-connection-throttling-4.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/email-connection-throttling-5.png)

儲存變更後，所有使用者都會將電子郵件批次傳送至其連線的Gmail或[!DNL Exchange]帳戶以進行傳遞。

## 電子郵件提供者限制 {#email-provider-limits}

**[!DNL Outlook 365]**

商業/企業

* 每天10,000
* 每分鐘30次
* 每封電子郵件500位收件者

如需詳細資訊[，請參閱此處](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)。

**Gmail**

* 每天2000個（試用和標幟帳戶為500個）
* 每秒2封電子郵件（API限制）
* 每則訊息2,000位收件者（外部收件者最多500位）

如需詳細資訊[，請參閱此處](https://support.google.com/a/answer/166852?hl=en)。

**[!DNL Microsoft Exchange Server (2010, 2013)]**

限制由組織的IT部門設定，因為伺服器由組織託管。 如有其他資訊，請聯絡網路或系統管理員。

>[!MORELIKETHIS]
>
>* [傳遞管道總覽](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* Gmail使用者的[電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [位使用者的 [!DNL Outlook] 電子郵件連線](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
