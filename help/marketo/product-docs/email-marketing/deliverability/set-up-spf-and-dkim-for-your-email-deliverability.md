---
unique-page-id: 4720710
description: 設定電子郵件傳遞的SPF和DKIM - Marketo檔案 — 產品檔案
title: 設定SPF和DKIM以傳遞電子郵件
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: de32becbfe74c2a88c53de8af8be4ee022782114
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 設定SPF和DKIM以傳遞電子郵件 {#set-up-spf-and-dkim-for-your-email-deliverability}

改善電子郵件傳送率的一個快速方法是 **SPF** （發件人策略框架）和 **DKIM** （已識別的網域金鑰郵件）放入您的DNS設定中。 除了DNS項目之外，您還告訴收件者您已授權Marketo代表您傳送電子郵件。 若未進行此變更，因為電子郵件是從您的網域寄送，但是從具有Marketo網域的IP位址傳送，因此您的電子郵件被標示為垃圾訊息的機率會較高。

>[!CAUTION]
>
>您需要您的網路管理員在DNS記錄中進行此更改。

## 設定SPF {#set-up-spf}

**如果您的域上沒有SPF記錄**

請您的網路管理員將下列行新增至DNS項目。 取代 [網域] 與網站的主網域(例如 &quot;company.com&quot;)和 [corpIP] 與公司電子郵件伺服器的IP位址(例如 &quot;255.255.255.255&quot;). 如果您透過Marketo從多個網域傳送電子郵件，應將此欄位新增至每個網域（一行）。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**如果您的網域上確實有SPF記錄**

如果DNS項中已有SPF記錄，請向其添加以下內容：

包括：mktomail.com

## 設定DKIM {#set-up-dkim}

**什麼是DKIM? 為什麼要設定DKIM?**

DKIM是驗證通訊協定，電子郵件接收者用來判斷電子郵件訊息是否是由其聲稱的傳送者所傳送。 DKIM通常可改善電子郵件傳送至收件匣的能力，因為接收者可以確信訊息並非偽造。

**DKIM是怎麼工作的？**

在您設定DNS記錄中的公開金鑰，並在「管理員」區段中啟用傳送網域(A)後，我們會開啟您傳出訊息的自訂DKIM簽署功能，其中包含加密的數位簽名，以及我們為您傳送的每封電子郵件(B)。 接收者將可在您的傳送網域的DNS(C)中查詢「公開金鑰」，以解密數位簽章。 如果電子郵件中的金鑰與您DNS記錄中的金鑰相對應，則接收郵件伺服器將更有可能接受代表您傳送的電子郵件Marketo。

![](assets/image2015-1-12-13-3a56-3a55.png)

**如何設定DKIM?**

請參閱 [設定自訂DKIM簽名](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md).

>[!MORELIKETHIS]
>
>* [了解SPF及其運作方式的更多資訊](http://www.open-spf.org/Introduction/)
>* [Marketo的電子郵件傳遞工具](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [我的SPF設定正確嗎？](https://www.kitterman.com/spf/validate.html)
>* [我使用正確的語法嗎？](http://www.open-spf.org/SPF_Record_Syntax/)

