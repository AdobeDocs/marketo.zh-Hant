---
unique-page-id: 4720433
description: 設定Marketo的通訊協定 — Marketo檔案 — 產品檔案
title: 設定Marketo的通訊協定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 3%

---

# 設定Marketo的通訊協定 {#configure-protocols-for-marketo}

如果您或您的組織使用限制性的防火牆或Proxy伺服器設定，您或您的網路管理員可能需要將某些網域和IP位址範圍列入允許清單，以確保Adobe Marketo Engage如預期般運作。

## 品牌行銷活動登陸頁面和電子郵件 {#branded-campaign-landing-pages-and-emails}

您的行銷團隊正在使用Marketo建立品牌行銷活動登入頁面和電子郵件。 為確保這些登入頁面和電子郵件正常運作，他們需要IT人員的協助。 請設定下列通訊協定，並提供行銷群組應傳送電子郵件給您的資訊。

本文內容應與希望實作這些通訊協定之公司的IT部門分享。

如果您的IT團隊限制使用允許清單進行網頁存取，請要求他們新增下列網域（包括星號），以允許所有Marketo資源和網頁通訊端：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`

## 步驟1：建立登入頁面和電子郵件的DNS記錄 {#step-create-dns-records-for-landing-pages-and-email}

**追蹤連結CNAME**

您的行銷團隊應傳送兩則新CNAME記錄的請求給您。 第一個是用於登入頁面URL，讓登入頁面以可反映您網域而非Marketo （實際主機）的URL顯示。 第二個是追蹤從Marketo傳送之電子郵件中所包含的連結。

`1` **為登陸頁面新增CNAME**

新增他們傳送給您的登陸頁面CNAME至您的DNS記錄，以便 `[YourLandingPageCNAME]` 指向指派給您Marketo登陸頁面的唯一帳戶字串。 登入您的網域註冊機構的網站，然後輸入登陸頁面CNAME和帳戶字串。 這通常涉及三個欄位：

* 別名：輸入 `[YourLandingPageCNAME]` （由行銷提供）
* 型別： CNAME
* 指向：輸入 `[MunchkinID].mktoweb.com` （由行銷提供）

`2` **新增電子郵件追蹤連結的CNAME**

新增行銷傳送給您的電子郵件CNAME，以便 `[YourEmailCNAME]` 指向 [MktoTrackingLink]，Marketo指派的預設追蹤連結，格式為：\
`[YourEmailCNAME].[YourDomain].com` 在CNAME中 `[MktoTrackingLink]`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` 必須是預設品牌定義域。

`3` **通知您的行銷團隊**

當您完成此程式時，請通知您的行銷團隊。

`4` **連絡人 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} 開始布建SSL憑證的程式。**

此程式最多可能需要3個工作日才能完成。

## 步驟2：允許列出Marketo IP {#step-allowlist-marketo-ips}

當您的行銷群組使用Marketo傳送測試電子郵件（傳送電子郵件爆炸訊息之前的最佳實務）時，測試電子郵件有時會遭到反垃圾郵件系統的封鎖，依賴寄件者IP位址來驗證電子郵件是否有效。 為確保這些測試電子郵件送達，請將Marketo新增至您的允許清單。

將這些IP位址新增至您的公司允許清單：

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

有些反垃圾郵件系統使用電子郵件傳迴路徑欄位來代替允許的IP位址。 在這些情況下，最好的辦法是將「&#42;.mktomail.com&#39;，因為Marketo使用數個信箱子網域。 其他反垃圾郵件系統根據寄件者地址加入允許清單。 在這些情況下，請務必加入您的行銷群組用來與人員/潛在客戶通訊的所有傳送（「寄件者」）網域。

>[!NOTE]
>
>Postini採用獨特的技術，並需要將IP範圍列入允許清單。 另請參閱 [使用Postini加入允許清單](https://nation.marketo.com/docs/DOC-1066).

## 步驟3：設定SPF和DKIM {#step-set-up-spf-and-dkim}

您的行銷團隊也應已將DKIM資訊傳送給您，以新增至您的DNS資源記錄（亦列於下方）。 依照步驟成功設定DKIM和SPF，然後通知您的行銷團隊這已更新。

1. 若要設定SPF，請在我們的DNS專案中新增下列行：

   `[CompanyDomain]` 在TXT中v=spf1 mx ip4：`[CorpIP]`\
   包含： mktomail.com ~all

   如果我們的DNS專案已經有現有的SPF記錄，只需新增下列內容即可：\
   包含： mktomail.com

   將CompanyDomain取代為您網站的主網域(例如： 」`(company.com/)`「)和CorpIP，以及您企業電子郵件伺服器的IP位址(例如 &quot;255.255.255.255&quot;). 如果您要透過Marketo從多個網域傳送電子郵件，應讓IT人員為每個網域新增此行（一行）。

1. 針對DKIM，請為我們要設定的每個網域建立DNS資源記錄。 我們將簽署的每個網域的主機記錄和TXT值如下：

   `[DKIMDomain1]`：主機記錄為 `[HostRecord1]` 且TXT值為 `[TXTValue1]`.

   `[DKIMDomain2]`：主機記錄為 `[HostRecord2]` 且TXT值為 `[TXTValue2]`.

   遵循下列步驟後，針對您設定的每個DKIMDomain複製HostRecord和TXTValue [此處提供指示](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. IT人員完成此步驟後，別忘了在「管理員>電子郵件> DKIM」中驗證每個網域。

## 步驟4：設定您網域的MX記錄 {#step-set-up-mx-records-for-your-domain}

MX記錄可讓您接收寄送電子郵件至之網域的郵件，以處理回覆和自動回應。 如果您從公司網域傳送，則可能已設定此專案。 如果沒有，您通常可以將其設定為對應到您公司網域的MX記錄。

## 輸出IP位址 {#outbound-ip-addresses}

輸出連線是Marketo Engage代表您連線至網際網路上的伺服器。 與您合作或您自己的IT組織的一些合作夥伴/廠商可能會使用允許清單來限制對伺服器的存取。 若是如此，您必須提供Marketo Engage的輸出IP位址區塊，以新增至其允許清單。

**Webhook**

Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} 流程動作是在智慧行銷活動中執行，會向外部Web服務發出HTTP請求。 如果Web服務發佈者使用外部Web服務所在網路的防火牆上的允許清單，則發佈者必須將下列IP位址區塊新增至其允許清單。

**CRM同步**

Marketo Engage [Salesforce CRM同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} 是對CRM供應商所發佈API發出傳出HTTP請求的整合機制。 您必須確保您的IT組織不會封鎖下列任何IP位址區塊，使其無法存取您的CRM供應商API。

**Marketo Engage傳出IP位址區塊**

下表涵蓋進行傳出呼叫的所有Marketo Engage伺服器。 如果您正在設定任何IP允許清單、伺服器、防火牆、存取控制清單、安全性群組或協力廠商服務，以接收來自Marketo Engage的傳出連線，請使用下列清單。

<table>
 <tbody>
  <tr>
   <th>IP區塊（CIDR表示法）</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
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

<table>
 <tbody>
  <tr>
   <th>個人IP位址</th>
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

