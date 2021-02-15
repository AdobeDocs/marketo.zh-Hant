---
unique-page-id: 14746594
description: 設定SMTP伺服器——行銷文檔——產品文檔
title: 設定SMTP伺服器
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---


# 設定SMTP伺服器{#setting-up-an-smtp-server}

## 概述{#overview}

**什麼是SMTP伺服器？**

**簡**&#x200B;單 ****&#x200B;郵 ****&#x200B;件傳 ****&#x200B;輸協定，此伺服器負責發送出站郵件。當您從電子郵件用戶端傳送電子郵件時，您使用相同的服務來傳送電子郵件。

**為什麼要使用Sales Connect設定SMTP伺服器？**

它可讓您運用公司領域的聲譽和傳遞能力，而不需依賴他人。 我們的預設MSC伺服器是共用IP池的一部分，這意味著從共用信譽中發送。 我們強烈建議您的團隊使用Sales Connect建立自己的傳送渠道。

**銷售連接如何與我的SMTP伺服器一起發送？**

遵循[這些步驟](https://docs.marketo.com/x/ZgPh)。

![](assets/1.png)

`<pre><em>SMTP Server Setup Page in Sales Connect</em><br> </pre>` **我需要在電子郵件客戶端中設定任何內容嗎？**

就傳送渠道而言，否。 在您安裝我們的附加元件後，Sales Connect將運用您為傳送電子郵件所設定的相同傳送管道。

## 獲取SMTP憑據{#getting-the-smtp-credentials}

**如何獲取SMTP憑據？**

請連絡您的IT團隊，以瞭解貴公司使用哪些傳送管道來傳送電子郵件，以及如何存取您的SMTP憑證。 根據伺服器的配置方式，SMTP伺服器名稱或伺服器埠可能有一些自定義值。 如果您沒有專屬的IT團隊，請聯絡您的電子郵件供應商。

**如果我的公司使用Office365，我有哪些選擇？**

專業人員

* 易於設定
* 任何擁有Office365帳戶的用戶都可以訪問此SMTP伺服器

缺點

* 可以進行調節
* 每位使用者都必須自行設定
* 變更使用者的O365密碼會導致連線中斷

如果您使用Office365或Exchange Online，則可以使用一組標準憑據連接到SMTP伺服器。 請記住，Office365不是大量電子郵件傳送服務，不過這對於傳送一次性電子郵件非常有用。 在傳送大量電子郵件時，Office365可能會限制您的電子郵件，而這可能會導致傳送失敗。 要瞭解更多有關此資訊，請查看Microsoft在[上的文章，瞭解如何設定SMTP客戶端提交](https://support.office.com/en-us/article/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-365-69f58e99-c550-4274-ad18-c805d654b4c4)。

「您只能從一個電子郵件地址傳送，除非您的裝置可以儲存多個Office 365郵箱的登入憑證。 Office 365規定每分鐘傳送30封訊息的限制，以及每天10,000封收件者的限制。」

如果您決定使用Office365做為傳送管道，則需要輸入這些認證。 由於Office365使用使用者的電子郵件和密碼來連線，因此無法跨團隊使用相同的認證。

Microsoft與大量傳送

[按一](https://technet.microsoft.com/en-us/library/exchange-online-limits.aspx#RecipientLimits) 下這裡，瞭解如何在Office365中大量傳送。

Exchange Online需要傳送合法大量商業電子郵件的客戶（例如，客戶電子報）應使用專門從事這些服務的第三方供應商。」

**如果我的公司使用Gmail呢？**

如果您的團隊想要使用Gmail作為Sales Connect的傳遞渠道，則不需要獲得任何SMTP憑證。 Sales Connect可讓使用者透過我們的OAuth整合，存取其Gmail傳送通道。 使用者可將Sales Connect帳戶與Gmail整合，以啟用此功能。

![](assets/2.png)

**我是否可以與整個團隊共用相同的SMTP憑據？**

這取決於您使用的傳送渠道。 例如，Sparkpost等服務允許憑證以網域為基礎，因此任何以特定網域傳送的使用者都會經過驗證，才能透過該伺服器傳送。 如果是，則可以與團隊共用認證。

如果您要連接到Office365，則憑證是基於電子郵件地址的。 這表示只有建立連線的電子郵件地址會經過驗證，才能透過該傳送管道傳送電子郵件，因此憑證應&#x200B;**不**&#x200B;共用。

![](assets/3.png)
