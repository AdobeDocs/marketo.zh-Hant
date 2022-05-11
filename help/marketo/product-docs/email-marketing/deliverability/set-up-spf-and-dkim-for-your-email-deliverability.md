---
unique-page-id: 4720710
description: 設定電子郵件傳輸的SPF和DKIM -Marketo文檔 — 產品文檔
title: 為電子郵件提供功能設定SPF和DKIM
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: de32becbfe74c2a88c53de8af8be4ee022782114
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 為電子郵件提供功能設定SPF和DKIM {#set-up-spf-and-dkim-for-your-email-deliverability}

提高電子郵件發送率的一種快速方法是 **SPF** （發件人策略框架）和 **DKIM** （域密鑰標識郵件）。 通過添加此DNS條目，您會告訴收件人您已授權Marketo代表您發送電子郵件。 如果不進行此更改，則您的電子郵件被標籤為垃圾郵件的可能性更高，因為電子郵件是從您的域發送的，但是是從具有Marketo域的IP地址發送的。

>[!CAUTION]
>
>您需要網路管理員在DNS記錄中進行此更改。

## 設定SPF {#set-up-spf}

**如果域上沒有SPF記錄**

請讓網路管理員將以下行添加到DNS條目。 替換 [域] 主域(例如 &quot;company.com&quot;和 [公司IP] 公司電子郵件伺服器的IP地址(例如 「255.255.255.255」)。 如果您通過Marketo從多個域發送電子郵件，則應將此內容添加到每個域（在一行上）。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**如果域上確實有SPF記錄**

如果您的DNS條目中已有SPF記錄，請向其添加以下內容：

包括：mktomail.com

## 設定DKIM {#set-up-dkim}

**什麼是DKIM? 為什麼要設定DKIM?**

DKIM是一種身份驗證協定，電子郵件接收者使用它來確定電子郵件是否由其說發送者發送。 DKIM通常會提高電子郵件到收件箱的傳送能力，因為接收者可以確信郵件不是偽造的。

**DKIM公司是如何工作的？**

在您在DNS記錄中設定公鑰並在「管理」部分(A)中激活發送域後，我們將為您的傳出消息啟用自定義DKIM簽名，其中將包括加密的數字簽名，並包含我們為您發送的每封電子郵件(B)。 接收方將能夠通過查找發送域DNS(C)中的「公鑰」來解密數字簽名。 如果電子郵件中的密鑰與DNS記錄中的密鑰相對應，則接收郵件伺服器更有可能接受Marketo代表您發送的電子郵件。

![](assets/image2015-1-12-13-3a56-3a55.png)

**如何設定DKIM?**

請參閱 [設定自定義DKIM簽名](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)。

>[!MORELIKETHIS]
>
>* [瞭解有關SPF及其工作原理的詳細資訊](http://www.open-spf.org/Introduction/)
>* [Marketo的電子郵件傳遞工具](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [我的SPF設定正確嗎？](https://www.kitterman.com/spf/validate.html)
>* [我使用了正確的語法嗎？](http://www.open-spf.org/SPF_Record_Syntax/)

