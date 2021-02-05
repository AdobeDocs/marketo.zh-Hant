---
unique-page-id: 4720710
description: 為您的電子郵件傳遞能力設定SPF和DKIM —— 行銷人員檔案——產品檔案
title: 設定SPF和DKIM以實現電子郵件傳遞
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---


# 為電子郵件傳遞能力設定SPF和DKIM {#set-up-spf-and-dkim-for-your-email-deliverability}

提高電子郵件傳送率的一個快速方法是將&#x200B;**SPF**（發件人策略框架）和&#x200B;**DKIM**（域密鑰標識郵件）合併到DNS設定中。 除了DNS項目外，您還告訴收件者您已授權Market代表您傳送電子郵件。 若未進行此變更，您的電子郵件自您的網域寄送，但是從具有Marketo網域的IP位址傳送，因此更容易被標示為垃圾訊息。

>[!CAUTION]
>
>您需要網路管理員在您的DNS記錄中進行此更改。

## 設定SPF {#set-up-spf}

**如果您的域上沒有SPF記錄**

請您的網路管理員將下列行新增至您的DNS項目。 將[domain]取代為網站的主網域(例如 &quot;company.com&quot;)和[corpIP]，以及您公司電子郵件伺服器的IP位址(例如 &quot;255.255.255.255&quot;)。 如果您透過Marketo從多個網域傳送電子郵件，您應將此電子郵件新增至每個網域（在一行）。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**如果您的域上有SPF記錄**

如果您的DNS條目中已經有SPF記錄，請在其中添加以下內容：

include:mktomail.com

## 設定DKIM {#set-up-dkim}

**什麼是DKIM?為什麼要設定DKIM?**

DKIM是一種驗證通訊協定，電子郵件接收者會使用此通訊協定來判斷電子郵件訊息是由誰傳送。 DKIM通常會改善電子郵件傳送至收件匣的能力，因為接收者可以確信訊息並非偽造。

**DKIM公司的運作方式為何？**

當您在DNS記錄中設定公開金鑰並啟用「管理」區段(A)中的傳送網域後，我們會為您的傳出訊息開啟自訂DKIM簽名，其中會包含加密的數位簽名，每封我們寄給您的電子郵件都會包含此簽名(B)。 接收者將可在您的傳送網域的DNS(C)中尋找「公開金鑰」來解密數位簽名。 如果電子郵件中的金鑰與您DNS記錄中的金鑰相符，則接收郵件伺服器將更有可能接受代您傳送的電子郵件行銷人員。

![](assets/image2015-1-12-13-3a56-3a55.png)

**我要如何設定DKIM?**

請參閱[設定自訂DKIM簽名](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)。

>[!MORELIKETHIS]
>
>* [進一步瞭解SPF及其運作方式](https://www.open-spf.org/Introduction/)
>* [Marketo的電子郵件傳遞能力工具](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [我的SPF設定正確嗎？](https://www.kitterman.com/spf/validate.html)
>* [我使用正確的語法嗎？](https://www.open-spf.org/SPF_Record_Syntax/)

