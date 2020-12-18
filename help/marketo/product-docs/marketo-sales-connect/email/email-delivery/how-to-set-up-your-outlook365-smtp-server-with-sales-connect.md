---
unique-page-id: 14352600
description: 如何使用銷售連接設定Outlook365 SMTP伺服器——行銷人員文檔——產品文檔
title: 如何使用Sales Connect設定Outlook365 SMTP伺服器
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# 如何使用Sales Connect {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}設定Outlook365 SMTP伺服器

>[!NOTE]
>
>如果您的組織使用Outlook，而您正嘗試使用Marketo Sales Connect設定電子郵件傳送渠道，我們建議使用我們的電子郵件連線功能[連線至您的Exchange伺服器。](http://docs.marketo.com/x/Z4AOAQ)

為了將自定義[SMTP](http://docs.marketo.com/x/zYTS)伺服器設定為備用傳送通道，ToutApp確實要求您出於安全考慮使用某種形式的驗證。 您可以在[SMTP配置頁](http://toutapp.com/next#settings/email-servers/smtp/configure)上設定任何SMTP伺服器。 要設定Office365 SMTP伺服器，Microsoft建議進行以下配置：\
**SMTP伺服器**:smtp.office365.com\
**伺服器埠**:埠587 —— 安全\
**驗證方法**:登入(SSL/TLS)\
**使用者名稱或登入**:您的Office365電子郵件地址\
**密碼**:您的Office365電子郵件密碼\
**您的網域**:您的公司網域

如果您仍然在設定SMTP伺服器時遇到問題，請與Exchange管理員合作，以確保使用正確的憑據。

>[!NOTE]
>
>當透過Office365 SMTP傳送時，Microsoft會規定`limit of 30 messages sent per minute`，並限制每天10,000個收件者。 此外，您的團隊中希望通過Office365 SMTP伺服器發送電子郵件的`each member`將需要在其Sales Connect設定中使用自己的電子郵件地址和密碼來設定此設定。 根據Microsoft的Office365帳戶策略，選中此配置的設定&quot; `Make this deliverability channel to all my team members` `" will not work`的複選框。

