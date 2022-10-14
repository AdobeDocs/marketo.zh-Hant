---
unique-page-id: 4720433
description: 設定Marketo的通訊協定 — Marketo檔案 — 產品檔案
title: 設定Marketo的通訊協定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: 3d29cb4cf4af7d83a82d47cfd6b0c44d659ee82b
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 2%

---

# 設定Marketo的通訊協定 {#configure-protocols-for-marketo}

如果您或您的組織使用嚴格的防火牆或代理伺服器設定，則您或您的網路管理員可能需要允許列出特定網域和IP位址範圍，以確保Adobe Marketo Engage可如預期般運作。

## 品牌行銷活動登陸頁面和電子郵件 {#branded-campaign-landing-pages-and-emails}

您的行銷團隊正使用Marketo建立品牌化的行銷活動登陸頁面和電子郵件。 為確保這些登錄頁面和電子郵件正常運作，他們需要IT的一點協助。 請設定下列通訊協定，以及行銷群組應以電子郵件傳送給您的資訊。

本文應與希望執行這些協定的公司的IT部門分享。

>[!NOTE]
>
>如果您的IT團隊使用允許清單限制Web存取，請要求他們新增下列網域（包括星號）以允許所有Marketo資源和網路通訊端：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`

## 步驟1:建立登錄頁面和電子郵件的DNS記錄 {#step-create-dns-records-for-landing-pages-and-email}

**追蹤連結CNAME**

您的行銷團隊應已傳送兩個請求，要求您提供新CNAME記錄。 第一個是用於登錄頁面URL，這樣登錄頁面就會出現在反映您網域的URL中，而非Marketo（實際主機）。 第二個是追蹤連結，這些連結包含在他們從Marketo傳送的電子郵件中。

`1` **新增登錄頁面的CNAME**

新增將您傳送至DNS記錄的登錄頁面CNAME，以便 `[YourLandingPageCNAME]` 指向指派給您的Marketo登陸頁面的唯一帳戶字串。 登入您的網域註冊機構的網站，並輸入登陸頁面CNAME和帳戶字串。 通常，這包含三個欄位：

* 別名：輸入 `[YourLandingPageCNAME]` （由行銷提供）
* 類型：CNAME
* 指向：輸入 `[MarketoAccountString].mktoweb.com` （由行銷提供）

`2` **新增CNAME以用於電子郵件追蹤連結**

新增您寄送的電子郵件CNAME行銷，以便 `[YourEmailCNAME]` 指向 [MktoTrackingLink]，此為Marketo指派的預設追蹤連結，格式為：\
`[YourEmailCNAME].[YourDomain].com` 在CNAME中 `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` 必須是預設品牌網域。

`3` **通知行銷團隊**

完成此程式後，通知您的行銷團隊。

`4` **連絡人 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;}以開始布建SSL憑證的程式。**

此程式最多需要3個工作天才能完成。

## 步驟2:允許清單Marketo IP {#step-allowlist-marketo-ips}

當您的行銷群組使用Marketo傳送測試電子郵件時（在傳送電子郵件爆炸訊息前為最佳作法），測試電子郵件有時會遭到反垃圾郵件系統封鎖，而反垃圾郵件系統依賴寄件者IP位址來驗證電子郵件是否有效。 若要確保這些測試電子郵件送達，請將Marketo新增至您的允許清單。

將這些IP位址新增至您的公司允許清單：

199.15.212.0/22\
192.28.144.0/20 192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

某些反垃圾郵件系統使用電子郵件「回訪路徑」欄位，而非IP地址進行分配。 在這些情況下，最好的方法是允許列出「&#42;.mktomail.com`，因為Marketo使用數個信箱子網域。 其他反垃圾郵件系統允許根據發件人地址列出。 在這些情況下，請務必包含您的行銷群組用來與人員/銷售機會通訊的所有傳送（「寄件者」）網域。

>[!NOTE]
>
>Postini採用獨特的技術，需要列入允許的IP範圍。 請參閱 [允許與Postini](https://nation.marketo.com/docs/DOC-1066).

## 步驟3:設定SPF和DKIM {#step-set-up-spf-and-dkim}

您的行銷團隊也應將DKIM資訊傳送給您，以便新增至您的DNS資源記錄（也列於下方）。 請依照步驟成功設定DKIM和SPF，然後通知您的行銷團隊此項目已更新。

1. 要設定SPF，請將以下行添加到DNS項：

   `[CompanyDomain]` 在TXT v=spf1 mx ip4中：`[CorpIP]`\
   包括：mktomail.com ~all

   如果DNS項中已有SPF記錄，只需在其中添加以下內容：\
   包括：mktomail.com

   將CompanyDomain取代為網站的主要網域(例如：&quot;`(company.com/)`「)」和CorpIP，以及您公司電子郵件伺服器的IP位址(例如 「255.255.255.255」)。 如果您要透過Marketo從多個網域傳送電子郵件，請讓IT人員為每個網域新增此行（一行）。

1. 針對DKIM，為每個要設定的網域建立DNS資源記錄。 以下是我們要簽署的每個網域的主機記錄和TXT值：

   `[DKIMDomain1]`:主機記錄為 `[HostRecord1]` 而TXT值為 `[TXTValue1]`.

   `[DKIMDomain2]`:主機記錄為 `[HostRecord2]` 而TXT值為 `[TXTValue2]`.

   複製您遵循 [說明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target=&quot;_blank&quot;}。 在IT人員完成此步驟後，別忘了在「管理員>電子郵件> DKIM」中驗證每個網域。

## 步驟4:為域設定MX記錄 {#step-set-up-mx-records-for-your-domain}

MX記錄允許您接收發送到要發送電子郵件的域的郵件，以處理回復和自動響應程式。 如果您要從公司網域傳送，您可能已設定此設定。 如果沒有，通常可以將其設定為與公司域的MX記錄映射。

## 傳出IP位址 {#outbound-ip-addresses}

出站連線是代表您Marketo Engage至網際網路上的伺服器所建立。 與您合作的某些合作夥伴/廠商或您自己的IT組織，可能會使用允許清單來限制對伺服器的存取。 若是如此，您必須提供Marketo Engage傳出IP位址區塊以新增至允許清單。

**Webhook**

Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target=&quot;_blank&quot;}是外站整合機制。 當 [呼叫Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target=&quot;_blank&quot;}流量動作會在智慧型促銷活動中執行，會對外部Web服務發出HTTP要求。 如果Web服務發佈者在外部Web服務所在網路的防火牆上使用允許清單，則發佈者必須將下面列出的IP地址塊添加到允許清單中。

**CRM同步**

Marketo Engage [Salesforce CRM同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target=&quot;_blank&quot;}和 [Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target=&quot;_blank&quot;}是整合機制，會對您的CRM廠商發佈的API提出傳出HTTP要求。 您必須確保IT組織不會封鎖下列任何IP位址區塊，以免存取您的CRM廠商API。

**Marketo Engage傳出IP位址區塊**

下表涵蓋進行傳出呼叫的所有Marketo Engage伺服器。 如果要配置任何IP允許清單、伺服器、防火牆、訪問控制清單、安全組或第三方服務來接收來自Marketo Engage的傳出連接，請使用下面的清單。

<table>
 <tbody>
  <tr>
   <th>IP區塊（CIDR標籤法）</th>
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
   <tr>
   <td>185.28.196.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
 </tbody>
</table>

<table>
 <tbody>
  <tr>
   <th>個別IP位址</th>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
   <tr>
   <td>44.235.171.179</td>
  </tr>
   <tr>
   <td>35.165.244.220</td>
  </tr>
   <tr>
   <td>52.20.211.99</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
   <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
   <tr>
   <td>54.220.138.65</td>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
 </tbody>
</table>

