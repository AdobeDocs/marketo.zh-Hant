---
unique-page-id: 4720433
description: 配置Marketo通訊協定-Marketo文檔——產品文檔
title: 配置Marketo協定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# 配置Marketo{#configure-protocols-for-marketo}的協定

您的行銷團隊正使用Marketo來建立品牌化的促銷活動登陸頁面和電子郵件。 為確保這些登陸頁面和電子郵件能正常運作，他們需要IT的協助。 請設定下列通訊協定，以及行銷群組應以電子郵件寄送給您的資訊。

本文應與希望執行這些通訊協定的公司IT部門分享。

>[!NOTE]
>
>如果您的IT團隊使用allowlist限制Web存取，請要求他們新增下列網域（包括星號），以允許所有Marketo資源和Web Sockets:

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## 步驟1:建立著陸頁面的DNS記錄並以電子郵件傳送{#step-create-dns-records-for-landing-pages-and-email}

**追蹤連結CNAME**

您的行銷團隊應已傳送兩份新CNAME記錄的要求給您。 第一個是用於著陸頁面URL，因此著陸頁面會顯示在反映您網域的URL中，而非Marketo（實際主機）。 第二個是追蹤連結，這些連結包含在他們從Marketo寄送的電子郵件中。

`1` **新增著陸頁面的CNAME**

新增他們將您傳送至DNS記錄的著陸頁面CNAME，讓`[YourLandingPageCNAME]`指向指派給您Marketo著陸頁面的唯一帳戶字串。 登入您的網域註冊機構網站，並輸入登陸頁面CNAME和帳戶字串。 通常，這涉及三個欄位：

* 別名：輸入`[YourLandingPageCNAME]`（由行銷部門提供）
* 類型：CNAME
* 指向：輸入`[MarketoAccountString].mktoweb.com`（由行銷部門提供）

`2` **新增電子郵件追蹤連結的CNAME**

新增您寄送的電子郵件CNAME行銷，讓`[YourEmailCNAME]`指向[MktoTrackingLink](Marketo指派的預設追蹤連結)，格式為：\
`[YourEmailCNAME].[YourDomain].com` 在CNAME中  `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **通知您的行銷團隊**

當您完成此程式時，通知您的行銷團隊。

## 步驟2:允許列出MarketoIP {#step-allowlist-marketo-ips}

當您的行銷群組使用Marketo傳送測試電子郵件（在發送電子郵件爆炸之前的最佳做法）時，測試電子郵件有時會被反垃圾郵件系統封鎖，這些系統依賴傳送者IP位址來驗證電子郵件是否有效。 為確保這些測試電子郵件送達，請將Marketo加入您的允許名單。

將這些IP位址新增至您的公司允許清單：

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

有些反垃圾郵件系統會使用電子郵件傳迴路徑欄位，而非IP位址進行分配。 在這些情況下，最好的方法是允許列出「*.mktomail.com」，因為Marketo使用多個郵箱子域。 其他反垃圾郵件系統允許根據「發件人」地址列出。 在這些情況下，請務必包含您的行銷群組用來與人員／潛在客戶通訊的所有傳送（「寄件者」）網域。

>[!NOTE]
>
>Postini採用獨特的技術，需要允許IP範圍。 請參閱[允許使用Postini](https://nation.marketo.com/docs/DOC-1066)。

## 步驟3:設定SPF和DKIM {#step-set-up-spf-and-dkim}

您的行銷團隊也應已傳送DKIM資訊給您，以便新增至您的DNS資源記錄（也列於下方）。 請依照步驟成功設定DKIM和SPF，然後通知您的行銷團隊此項更新已完成。

1. 要設定SPF，請將以下行添加到我們的DNS條目：

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   包括：mktomail.com ~all

   如果我們的DNS條目中已有SPF記錄，只需在其中添加以下內容：\
   包括：mktomail.com

   將CompanyDomain取代為您網站的主網域(例如：&quot;`(company.com/)`&quot;)和CorpIP，以及您公司電子郵件伺服器的IP位址(例如 &quot;255.255.255.255&quot;)。 如果您要透過Marketo從多個網域傳送電子郵件，您的IT人員應為每個網域（在一行）新增此行。

1. 對於DKIM，請為每個要設定的域建立DNS資源記錄。 以下是我們將簽署的每個網域的主機記錄和TXT值：

   `[DKIMDomain1]`:主機記錄 `[HostRecord1]` 為，TXT值為 `[TXTValue1]`。

   `[DKIMDomain2]`:主機記錄 `[HostRecord2]` 為，TXT值為 `[TXTValue2]`。

   按照[此處](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)的說明，複製您所設定的每個DKIMDomain的HostRecord和TXTValue。 在您的IT人員完成此步驟後，別忘了在「管理員>電子郵件> DKIM」中驗證每個網域。

## 步驟4:為域{#step-set-up-mx-records-for-your-domain}設定MX記錄

MX記錄可讓您接收電子郵件至您要傳送電子郵件的網域，以處理回覆和自動回覆者。 如果您是從公司網域傳送，則可能已設定此設定。 若未設定，您通常可設定它以對應至您公司網域的MX記錄。
