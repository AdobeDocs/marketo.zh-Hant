---
unique-page-id: 14352407
description: 傳送渠道概觀——行銷人員檔案——產品檔案
title: 傳送渠道概觀
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# 傳送渠道概述{#delivery-channel-overview}

我們將分析您可運用的3種不同通道、如何選擇它們、何時選擇一個通道，以及它們的細微差別。

>[!NOTE]
>
>只有當您從[Web應用程式](https://toutapp.com/login)傳送電子郵件時，才會有這項資訊。 如果您在Gmail或Outlook中使用Sales Connect，您的電子郵件會透過這些電子郵件伺服器傳送。

## MSC電子郵件伺服器（預設）{#msc-email-servers-default}

依預設，系統會選取此方法來傳送您的電子郵件。 MSC電子郵件伺服器是不使用Gmail或Outlook的使用者的絕佳選擇。 此外，由於它們是我們的伺服器，因此我們能夠接收任何有關彈回或交付失敗的錯誤消息，並在「對話」頁籤的「交付失敗」部分將其呈現給您。

使用MSC伺服器的另一個好處是，當使用[電子郵件身份](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/add-identity.md)時，收件人將看到您建立的身份的電子郵件地址。

當使用MSC伺服器時，您的收件者可能會看到「via toutapp.com」標籤。 這是他們的電子郵件客戶，讓他們知道電子郵件是使用Sales Connect傳送的。

如需詳細資訊，請參閱[Gmail說明文章](https://support.google.com/mail/answer/1311182?hl=en)。

>[!NOTE]
>
>我們的MSC伺服器沒有提供的[DMARC記錄](https://dmarc.org/)。 您自己的伺服器上無法將它們列入白名單。

## Gmail伺服器{#gmail-server}

如果貴公司的電子郵件提供者是Gmail，您可以利用現有帳戶傳送Sales Connect電子郵件。 如果您想要避免「透過toutapp.com」資訊，而且希望仰賴公司網域的聲譽和傳遞能力，這是絕佳的選擇。 使用Gmail伺服器的另一個好處是，從Web應用程式發送的任何內容都會自動添加到Gmail發送資料夾。

我們只能正確連接一個Gmail帳戶（一個電子郵件地址），以傳遞您的Sales Connect電子郵件。 這表示如果您使用多個電子郵件身分識別，當查看詳細資訊時，只會顯示我們所連線之帳戶的位址。

在Web應用程式中，您的身分將會像您所建立的一樣顯示（上圖）。 但是，通過Gmail伺服器發送郵件時，會顯示連接帳戶的地址。

>[!NOTE]
>
>由於Sales Connect不直接管理您的Gmail伺服器，因此我們不會在Web應用程式中記錄跳回的電子郵件事件。

## 自定義SMTP伺服器{#custom-smtp-server}

為您自己的伺服器付費？ 使用Microsoft Exchange環境？ 這是您的選擇。 請參閱[這些有關設定的說明](https://docs.marketo.com/x/zYTS)。 與Gmail伺服器一樣，由於Sales Connect不直接管理您的伺服器，因此我們不會在Web應用程式中記錄跳回的電子郵件事件。
