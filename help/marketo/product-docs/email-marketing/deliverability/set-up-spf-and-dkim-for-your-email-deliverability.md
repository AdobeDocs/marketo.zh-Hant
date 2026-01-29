---
unique-page-id: 4720710
description: 設定 SPF 和 DKIM 以確保電子郵件傳遞能力 - Marketo 文件 — 產品文件
title: 設定 SPF 和 DKIM 以確保電子郵件傳遞能力
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '421'
ht-degree: 100%

---

# 設定 SPF 和 DKIM 以確保電子郵件傳遞能力 {#set-up-spf-and-dkim-for-your-email-deliverability}

提升電子郵件傳遞率的快速方法之一就是將 **SPF** (寄件者原則架構) 和 **DKIM** (Domain Keys Identified Mail) 納入您的 DNS 設定。透過在 DNS 項目中新增此內容，可通知收件者，您已授權 Marketo 代表您傳送電子郵件。若未進行此變更，您的電子郵件被標記為垃圾郵件的可能性會較高，因為電子郵件雖然顯示寄件網域為您的網域，但實際卻是由 Marketo 網域的 IP 位址傳送。

>[!CAUTION]
>
>您需要請網路管理員在 DNS 記錄中進行此變更。

## 設定 SPF {#set-up-spf}

**如果您的網域沒有 SPF 記錄**

請要求您的網路管理員將下行新增到您的 DNS 項目中。將[網域]替換為您網站的主網域 (例如： 「company.com」)，並將 [corpIP] 替換為貴公司電子郵件伺服器的 IP 位址 (例如：「255.255.255.255」)。如果您透過 Marketo 從多個網域傳送電子郵件，應將此新增至每個網域 (在同一行)。

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**如果您的網域中確實存在 SPF 記錄**

如果您的 DNS 項目中已經有 SPF 記錄，則請在其中新增以下內容：

include:mktomail.com

## 設定 DKIM {#set-up-dkim}

**什麼是 DKIM？為什麼要設定 DKIM？**

DKIM 是一種驗證通訊協定，電子郵件接收者會將其用於確定電子郵件是否真由聲稱的寄件者所傳送。DKIM 通常可提升電子郵件至收件匣的傳遞能力，因為接收者可確信該訊息並非偽造。

**DKIM 如何運作？**

您在 DNS 記錄中設定公開金鑰並在「管理員」區段中啟用傳送網域後 (A)，我們即會為您的傳出訊息開啟自訂 DKIM 簽署，其中包括我們為您傳送的每封電子郵件的加密數位簽名 (B)。接收者即可透過在傳送網域的 DNS 中查詢「公開金鑰」將數位簽名解密 (C)。如果電子郵件中的金鑰與您 DNS 記錄中的金鑰相對應，則接收郵件伺服器即更有可能接受 Marketo 代表您傳送的電子郵件。

![](assets/image2015-1-12-13-3a56-3a55.png)

**如何設定 DKIM？**

請參閱[設定自訂 DKIM 簽名](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}。

>[!MORELIKETHIS]
>
>* 了解更多 SPF 及其運作方式的資訊`: http://www.open-spf.org/Introduction/`
>* 我的 SPF 設定是否正確？：`https://www.kitterman.com/spf/validate.html`
>* 我是否使用正確的語法？：`http://www.open-spf.org/SPF_Record_Syntax/`
