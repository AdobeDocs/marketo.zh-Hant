---
unique-page-id: 4720710
description: 針對您的電子郵件傳遞能力設定SPF和DKIM - Marketo檔案 — 產品檔案
title: 設定SPF和DKIM以提供電子郵件傳遞能力
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 設定SPF和DKIM以提供電子郵件傳遞能力 {#set-up-spf-and-dkim-for-your-email-deliverability}

提高電子郵件傳送率的一種快速方法是納入 **SPF** （寄件者原則架構）及 **DKIM** （網域金鑰識別郵件）放入您的DNS設定中。 除了您的DNS專案以外，您也會告訴收件者，您已授權Marketo代表您傳送電子郵件。 若沒有此變更，則您的電子郵件被標示為垃圾郵件的可能性會較高，因為電子郵件是從您的網域寄出，但是從具有Marketo網域的IP位址傳送。

>[!CAUTION]
>
>您需要網路系統管理員才能在DNS記錄中進行此變更。

## 設定SPF {#set-up-spf}

**如果您的網域中沒有SPF記錄**

請要求您的網路管理員將以下行新增到您的DNS專案中。 取代 [網域] 與網站的主要網域(例如 &quot;company.com&quot;)和 [corpIP] ，並使用公司電子郵件伺服器的IP位址(例如 &quot;255.255.255.255&quot;). 如果您透過Marketo從多個網域傳送電子郵件，應將此專案新增至每個網域（一行）。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**如果您的網域中確實有SPF記錄**

如果您的DNS專案中已有SPF記錄，請新增下列內容：

包含：mktomail.com

## 設定DKIM {#set-up-dkim}

**什麼是DKIM？ 為什麼我要設定DKIM？**

DKIM是一種驗證通訊協定，電子郵件接收者會使用該通訊協定來判斷電子郵件訊息的傳送者是否是其聲稱的傳送者。 DKIM通常可改善將電子郵件傳送至收件匣的能力，因為接收者可以確信郵件並非偽造。

**DKIM如何運作？**

當您在DNS記錄中設定公開金鑰並在Admin區段中啟用傳送網域後(A)，我們會針對您的傳出郵件開啟自訂DKIM簽署，其中包括我們為您傳送的每封電子郵件的加密數位簽名(B)。 接收者將透過在傳送網域的DNS (C)中查詢「公開金鑰」來解密數位簽名。 如果電子郵件中的金鑰與您DNS記錄中的金鑰相對應，則接收郵件伺服器將更有可能接受代表您傳送的電子郵件Marketo。

![](assets/image2015-1-12-13-3a56-3a55.png)

**如何設定DKIM？**

請參閱 [設定自訂DKIM簽章](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [進一步瞭解SPF及其運作方式](http://www.open-spf.org/Introduction/){target="_blank"}
>* [我的SPF設定是否正確？](https://www.kitterman.com/spf/validate.html){target="_blank"}
>* [我是否使用正確的語法？](http://www.open-spf.org/SPF_Record_Syntax/){target="_blank"}
