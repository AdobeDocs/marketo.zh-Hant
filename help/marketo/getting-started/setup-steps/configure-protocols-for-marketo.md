---
unique-page-id: 4720433
description: 配置Marketo協定 — Marketo文檔 — 產品文檔
title: 配置Marketo協定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---

# 配置Marketo協定 {#configure-protocols-for-marketo}

如果您或您的組織使用限制性防火牆或代理伺服器設定，則您或您的網路管理員可能需要允許列出某些域和IP地址範圍，以確保Adobe Marketo Engage按預期工作。

## 品牌活動登錄頁和電子郵件 {#branded-campaign-landing-pages-and-emails}

您的營銷團隊正在使用Marketo建立品牌營銷活動登錄頁和電子郵件。 為確保這些登錄頁和電子郵件能夠正常工作，他們需要IT部門提供一些幫助。 請設定以下協定，並提供營銷小組應通過電子郵件向您發送的資訊。

本文應與希望實施這些協定的公司的IT部門分享。

>[!NOTE]
>
>如果您的IT團隊使用允許清單限制Web訪問，請要求他們添加以下域（包括星號）以允許所有Marketo資源和Web套接字：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`

## 步驟1:為登錄頁和電子郵件建立DNS記錄 {#step-create-dns-records-for-landing-pages-and-email}

**跟蹤連結CNAME**

您的營銷團隊應已向您發送了兩個新CNAME記錄的請求。 第一種是登錄頁URL，以便登錄頁顯示在反映您的域的URL中，而不是Marketo（實際主機）。 第二個是追蹤連結，這些連結包含在他們從Marketo發送的電子郵件中。

`1` **為登錄頁添加CNAME**

添加登錄頁CNAME，它們將您發送給DNS記錄，以便 `[YourLandingPageCNAME]` 指向分配給您的Marketo登錄頁的唯一帳戶字串。 登錄到域註冊機的站點，然後輸入登錄頁CNAME和帳戶字串。 通常，這涉及三個欄位：

* 別名：輸入 `[YourLandingPageCNAME]` （由營銷提供）
* 類型：名稱
* 指向：輸入 `[MarketoAccountString].mktoweb.com` （由營銷提供）

`2` **為電子郵件跟蹤連結添加CNAME**

添加已發送給您的電子郵件CNAME營銷，以便 `[YourEmailCNAME]` 指向 [MktoTrackingLink],Marketo指定的預設跟蹤連結，格式為：\
`[YourEmailCNAME].[YourDomain].com` 在名稱中 `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **通知您的營銷團隊**

完成此過程後通知您的營銷團隊。

`4` **聯繫人 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;}以啟動設定SSL證書的過程。**

此過程最多需要3個工作日才能完成。

## 步驟2:允許清單MarketoIP {#step-allowlist-marketo-ips}

當您的營銷組使用Marketo發送test電子郵件（在發送電子郵件爆炸之前的最佳做法）時，test電子郵件有時會被反垃圾郵件系統阻止，這些系統依賴發送方IP地址來驗證電子郵件是否有效。 要確保這些test電子郵件到達，請將Marketo添加到您的允許清單。

將以下IP地址添加到公司允許清單：

199.15.212.0/22\
192.28.144.0/20 192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

某些反垃圾郵件系統使用電子郵件返迴路徑欄位而不是IP地址進行分配。 在這些情況下，最好的方法是允許&#42;.mktomail.com」，因為Marketo使用多個郵箱子域。 其他反垃圾郵件系統允許基於發件人地址列出。 在這些情況下，請確保包括您的市場營銷組用於與人員/線索通信的所有發送（「發件人」）域。

>[!NOTE]
>
>Postini採用一種獨特的技術，需要允許IP範圍。 請參閱 [允許與Postini](https://nation.marketo.com/docs/DOC-1066)。

## 第3步：設定SPF和DKIM {#step-set-up-spf-and-dkim}

您的營銷團隊應該還向您發送了要添加到DNS資源記錄的DKIM資訊（也列於下面）。 按照步驟成功配置DKIM和SPF，然後通知您的營銷團隊此操作已更新。

1. 要設定SPF，請將以下行添加到我們的DNS條目：

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   包括：mtomail.com ~all

   如果我們的DNS條目中已有SPF記錄，只需將以下內容添加到該條目：\
   包括：mtomail.com

   將CompanyDomain替換為網站的主域(例如：&quot;`(company.com/)`「 」)和CorpIP ，其IP地址為公司電子郵件伺服器(例如 「255.255.255.255」)。 如果您要通過Marketo從多個域發送電子郵件，您應讓您的IT人員為每個域（在一行上）添加此行。

1. 對於DKIM，為要設定的每個域建立DNS資源記錄。 下面是我們將為其簽名的每個域的主機記錄和TXT值：

   `[DKIMDomain1]`:主機記錄為 `[HostRecord1]` TXT值為 `[TXTValue1]`。

   `[DKIMDomain2]`:主機記錄為 `[HostRecord2]` TXT值為 `[TXTValue2]`。

   在以下操作之後，複製您設定的每個DKIMDomain的HostRecord和TXTValue [說明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target=&quot;_blank&quot;}。 在IT人員完成此步驟後，不要忘記在「管理」>「電子郵件」>「DKIM」中驗證每個域。

## 第4步：設定域的MX記錄 {#step-set-up-mx-records-for-your-domain}

MX記錄允許您將郵件發送到您正在發送的域以處理回復和自動應答。 如果您正從公司域發送，則可能已配置了此功能。 否則，您通常可以設定它以映射到您公司域的MX記錄。

## 出站IP地址 {#outbound-ip-addresses}

出站連接是通過代表您Marketo Engage到Internet上的伺服器而建立的。 您與某些合作夥伴/供應商或您自己的IT組織合作，可能使用允許清單限制對伺服器的訪問。 如果是，則必須為他們提供Marketo Engage出站IP地址塊以添加到其允許清單。

**網鈎**

Marketo Engage [網鈎](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target=&quot;_blank&quot;}是出站整合機制。 當 [呼叫Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target=&quot;_blank&quot;}流操作作為智慧活動的一部分執行，向外部Web服務發出HTTP請求。 如果Web服務發佈者在外部Web服務所在的網路的防火牆上使用允許清單，則發佈者必須將下面列出的IP地址塊添加到其允許清單中。

**CRM同步**

Marketo Engage [Salesforce CRM同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target=&quot;_blank&quot;和 [Microsoft動力同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target=&quot;_blank&quot;}是整合機制，用於向CRM供應商發佈的API發出出站HTTP請求。 您必須確保您的IT組織不會阻止以下任何IP地址塊訪問您的CRM供應商API。

**Marketo Engage出站IP地址塊**

下表涵蓋進行出站呼叫的所有Marketo Engage伺服器。 如果要配置任何IP允許清單、伺服器、防火牆、訪問控制清單、安全組或第三方服務以從Marketo Engage接收傳出連接，請使用此清單。

<table>
 <tbody>
  <tr>
   <th>IP塊（CIDR表示法）</th>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
   <tr>
   <td>192.28.160.0/19</td>
  </tr>
   <tr>
   <td>199.15.212.0/22</td>
  </tr>
 </tbody>
</table>
