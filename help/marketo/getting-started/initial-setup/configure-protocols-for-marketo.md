---
unique-page-id: 4720433
description: 設定 Marketo Engage 的通訊協定 - Marketo Engage 文件 - 產品文件
title: 設定 Marketo Engage 的通訊協定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '2131'
ht-degree: 100%

---

# 設定 Marketo Engage 的通訊協定{#configure-protocols-for-marketo-engage}

如果您或您的組織使用限制性的防火牆或 Proxy 伺服器設定，您或您的網路管理員可能需要將特定網域與 IP 位址範圍加入允許清單，以確保 Adobe Marketo Engage 如預期般運作。

如需協助實作下列通訊協定，請和您的 IT 部門分享本文。如果他們使用允許清單來限制網頁存取，請確保他們新增以下網域 (包括星號)，以便允許所有 Marketo Engage 資源和 WebSocket：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## 步驟1：建立登陸頁面和電子郵件的 DNS 記錄 {#step-create-dns-records-for-landing-pages-and-email}

**追蹤連結 CNAME**

您的行銷團隊應傳送兩個新 CNAME 記錄的要求給您。第一個是用於登陸頁面 URL，讓登陸頁面以反映您網域的 URL 顯示，而非以 Marketo Engage (實際主機) 顯示。第二個用於追蹤從 Marketo Engage 傳送的電子郵件中所包含的連結。

`1` **為登陸頁面新增 CNAME**

將傳送給您的登陸頁面 CNAME 新增至您的 DNS 記錄，這樣 `[YourLandingPageCNAME]` 即會指向指派給您的 Marketo Engage 登陸頁面的唯一帳戶字串。登入您的網域註冊機構的網站，然後輸入登陸頁面 CNAME 和帳戶字串。這通常包含三個欄位：

* 別名：輸入 `[YourLandingPageCNAME]` (由行銷提供)
* 類型：CNAME
* 指向：輸入 `[MunchkinID].mktoweb.com` (由行銷提供)

`2` **新增電子郵件追蹤連結的 CNAME**

新增傳送給您的電子郵件 CNAME 行銷，這樣 `[YourEmailCNAME]` 即會指向 [MktoTrackingLink] (Marketo Engage 指派的預設追蹤連結)，格式為：`[MktoTrackingLink]`IN CNAME`[YourEmailCNAME].[YourDomain].com`

例如：

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` 必須是預設品牌化網域。

`3` **通知您的行銷團隊**

完成此流程時，請通知您的行銷團隊。

`4` **聯絡 [Adobe 支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}，以開始佈建 SSL 憑證的流程。**

此流程可能需要最多 3 個工作天才能完成。

## 步驟 2：將 Marketo Engage IP 加入允許清單 {#step-allowlist-marketo-ips}

您的行銷群組使用 Marketo Engage 來傳送測試電子郵件 (在傳送電子郵件群發前的最佳做法) 時，測試電子郵件有時會遭到反垃圾郵件系統封鎖，這些系統依賴寄件者 IP 位址來驗證電子郵件是否有效。為確保這些測試電子郵件順利送達，請將 Marketo Engage 新增至您的允許清單。

將這些 IP 位址新增至您的公司允許清單：

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

有些反垃圾郵件系統會使用電子郵件返回路徑 (Return-Path) 欄位而不是 IP 位址來設定允許清單。在這些情況下，最好的方法是將 &#39;&#42;.mktomail.com&#39; 加入允許清單，因為 Marketo Engage 會使用好幾個信箱子網域。其他反垃圾郵件系統則會根據寄件者地址來設定允許清單。在這些情況下，請務必包含您的行銷群組用來與人員/銷售線索通訊的所有傳送 (「寄件者」) 網域。

>[!NOTE]
>
>Postini 採用獨特技術，並要求將 IP 範圍加入允許清單。請參閱[使用 Postini 進行允許清單設定](https://nation.marketo.com/docs/DOC-1066)。

## 步驟 3：設定 SPF 和 DKIM {#step-set-up-spf-and-dkim}

您的行銷團隊應該已經傳送給您 DKIM (Domain Keys Identified Mail) 資訊，以便新增至您的 DNS 資源記錄 (如下所列)。依照下列步驟即可成功地設定 DKIM 和 SPF (寄件者原則框架)，然後在完成更新時會通知您的行銷團隊。

1. 若要設定 SPF，請將下面一行新增至我們的 DNS 項目：

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
include: mktomail.com ~all

   如果在我們的 DNS 項目中已經有現存的 SPF 記錄，則只需新增以下內容即可：include: mktomail.com

   將 CompanyDomain 以您的網站主網域 (例如 `(company.com/)`) 取代，並將 CorpIP 替換成您公司電子郵件伺服器的 IP 位址 (例如，「255.255.255.255」)。如果您要透過 Marketo Engage 從多個網域傳送電子郵件，請要求 IT 人員為每個網域新增此行 (在同一行)。

1. 若是 DKIM，請為每個我們要設定的網域建立 DNS 資源記錄。下列為我們將簽署的每個網域的主機記錄和 TXT 值：

   `[DKIMDomain1]`：主機記錄為 `[HostRecord1]`，TXT 值為 `[TXTValue1]`。

   `[DKIMDomain2]`：主機記錄為 `[HostRecord2]`，TXT 值為 `[TXTValue2]`。

   請依照[此處的指示](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}為您已設定的每個 DKIMDomain 複製 HostRecord 和 TXTValue。IT 人員完成此步驟後，別忘了在「管理員 > 電子郵件 > DKIM」中驗證每個網域。

## 步驟 4：設定 DMARC {#set-up-dmarc}

DMARC (Domain-based Message Authentication, Reporting &amp; Conformance) 是一種驗證通訊協定，用於協助組織保護其網域免於未經授權的使用。DMARC 可擴展現有的驗證通訊協定 (例如 SPF 和 DKIM)，以便在收件者的網域驗證失敗時，可通知收件者伺服器應採取什麼動作。雖然 DMARC 目前為選用項目，但強烈建議您使用，因為這樣可以為貴組織的品牌和聲譽提供更佳保護。Google 和 Yahoo 等主要供應商從 2024 年 2 月開始即要求大量郵件的寄件者使用 DMARC。

要讓 DMARC 正常運作，您必須至少擁有以下其中一項 DNS TXT 記錄：

* 有效的 SPF
* 為您的寄件者: 網域設定有效的 DKIM 記錄 (建議用於 Marketo Engage)。

此外，您必須為您的寄件者: 網域設定 DMARC 特定 DNS TXT 記錄。您可選擇定義您選擇的電子郵件地址，以指定組織內接收 DMARC 報告的位置，以便您監視報告。

以最佳做法而言，建議逐步推出 DMARC 實作，隨著您對 DMARC 潛在影響的理解逐漸加深，將 DMARC 原則從 p=none 提升為 p=quarantine，再到 p=reject，同時將 SPF 與 DKIM 的 DMARC 原則設定為「寬鬆比對」

### DMARC 範例工作流程 {#dmarc-example-workflow}

1. 如果系統已將您設定為接收 DMARC 報告，您應該進行下列步驟...

   I. 分析您收到的意見反應與報告並使用 (p=none)，這會告知接收者不要對驗證失敗的郵件執行任何動作，但仍將電子郵件報告傳送給寄件者。

   II. 如果合法郵件驗證失敗，請檢閱並修正 SPF/DKIM 的問題。

   III. 確定 SPF 或 DKIM 是否一致，且是否通過所有合法電子郵件的驗證。

   IV. 檢閱報告以確保結果符合您根據 SPF/DKIM 原則所預期的結果。

1. 繼續將原則調整為 (p=quarantine)，這會告知接收電子郵件的伺服器將未通過驗證的電子郵件隔離 (這通常表示將這些郵件放入垃圾郵件資料夾中)。

   I. 檢閱報告以確保結果符合您的預期。

1. 如果您對 p=quarantine 等級的郵件行為感到滿意，則可以將原則調整為 (p=reject)。p=reject 原則會告知接收者，對於驗證失敗的網域中的任何電子郵件，可完全拒絕 (退回)。啟用此原則後，只有確認為已經過網域 100% 驗證的電子郵件才有機會進入收件匣。

>[!CAUTION]
>
>謹慎使用此原則並確認其是否適合您的組織。

### DMARC 報告 {#dmarc-reporting}

DMARC 可以接收未通過 SPF/DKIM 驗證的電子郵件之報告。在驗證流程中，ISP 服務商會產生兩種不同的報告，寄件者可透過 DMARC 原則中的 RUA/RUF 標記來接收這些報告。

* 彙總報告 (RUA)：不包含任何可能屬於 GDPR (一般資料保護規範) 敏感資訊的 PII (個人識別資訊)。

* 鑑識報告 (RUF)：包含屬於 GDPR 敏感資訊的電子郵件地址。使用之前，最好從內部檢查如何處理需要符合 GDPR 的資訊。

這些報告的主要用途是讓您大致了解有哪些偽冒的電子郵件。這些報告含有大量技術知識，因此最好透過第三方工具來消化。

### DMARC 記錄範例 {#example-dmarc-records}

* 最低限度記錄：`v=DMARC1; p=none`

* 導向至電子郵件地址以便接收報告的記錄：`v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC 標記及其功用 {#dmarc-tags-and-what-they-do}

DMARC 記錄有多個組成部分，稱為 DMARC 標記。每個標記都有一個值，可用來指定 DMARC 的某個部分。

<table>
<thead>
  <tr>
    <th>標記名稱 </th>
    <th>必要/選用 </th>
    <th>功能 </th>
    <th>範例 </th>
    <th>預設值 </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>必要</td>
    <td>此 DMARC 標記會指定版本。目前只有一個版本，因此其固定值為 v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>必要</td>
    <td>顯示已選取的 DMARC 原則，並指示接收者報告、隔離或拒絕未通過驗證檢查的電子郵件。</td>
    <td>p=none、quarantine 或 reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>選用</td>
    <td>允許網域擁有者指定報告選項。</td>
    <td>0：如果一切失敗，則產生報告
    <br>1：如果發生任何失敗，則產生報告
    <br>d：如果 DKIM 失敗，則產生報告
    <br>s：如果 SPF 失敗，則產生報告</td>
    <td>1 (DMARC 報告建議使用)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>選用</td>
    <td>告知需要篩選之郵件的百分比。</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>選用 (建議)</td>
    <td>識別彙總報告的送達位置。</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>選用 (建議)</td>
    <td>識別鑑識報告的送達位置。</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>選用</td>
    <td>為上層網域的子網域指定 DMARC 原則。</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>選用</td>
    <td>可以是嚴格 (s) 或寬鬆 ®。寬鬆比對表示該網域用於 DKIM 簽章，並且可以是「寄件者」地址的子網域。嚴格比對表示用於 DKIM 簽章的網域必須和用於寄件者地址的網域完全相符。</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>選用</td>
    <td>可以是嚴格 (s) 或寬鬆 ®。寬鬆比對表示 ReturnPath 網域可以是寄件者地址的子網域。嚴格比對表示 Return-Path 網域必須和寄件者地址完全相符。</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

如需有關 DMARC 及其所有選項的完整詳細資料，請造訪 [https://dmarc.org/](https://dmarc.org/){target="_blank"}。

### DMARC 和 Marketo Engage {#dmarc-and-marketo-engage}

DMARC 有兩種比對類型：DMARC—DKIM 比對和 SPF 比對。

>[!NOTE]
>
>建議在 Marketo Engage 中，優先使用 DKIM 而非 SPF 來進行 DMARC 比對。

* 與 DKIM 比對的 DMARC - 若要設定與 DKIM 比對的 DMARC，您必須：

   * 為您的郵件的寄件者: 網域設定 DKIM。使用](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}本文中[的指示。
   * 為先前已設定的寄件者:/DKIM 網域設定 DMARC

* 與 DMARC 比對的 SPF - 若要透過具品牌識別的 return-path 來設定與 DMARC 比對的 SPF，您必須：

   * 設定具品牌識別的 Return-Path 網域
      * 設定適當的 SPF 記錄
      * 將 MX 記錄變更為指向傳送出您的郵件之資料中心的預設 MX

   * 設定具品牌識別的 Return-Path 網域之 DMARC

* 如果您透過專用 IP 從 Marketo Engage 傳送郵件，且尚未實作具品牌識別的 return-path 或不確定是否已實作，請向 [Adobe 支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}提交票證。

* 如果您透過共用 IP 集區從 Marketo Engage 傳送郵件，您可以透過[在此套用](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}來查看您是否符合受信任的 IP 資格。具品牌識別的 return-path 會免費提供給從 Marketo Engage 受信任的 IP 傳送的使用者。如果此方案獲得核准，請聯繫 Adobe 支援部門來設定具品牌識別的 return-path。

   * 受信任的 IP：IP 的共用集區，保留給每月寄送量低於 75,000 封、且不符合專用 IP 資格的少量使用者。這些使用者也必須滿足最佳做法的需求。

* 如果您透過共用 IP 從 Marketo Engage 傳送郵件，但不符合受信任的 IP 的資格，且每月傳送的郵件超過 100,000 封，則您需要和 Adobe 客戶團隊 (您的客戶經理) 聯絡，以購買專用 IP。

* 在 Marketo Engage 中，不支援也不建議使用嚴格的 SPF 比對。

## 步驟 5：設定您的網域的 MX 記錄 {#step-set-up-mx-records-for-your-domain}

MX 記錄可讓您在寄送電子郵件的網域上接收郵件，以便處理回覆與自動回覆。如果您正從公司網域傳送，則有可能已經完成此設定。如果沒有，您通常可以將其設定為對應至您公司網域的 MX 記錄。

## 傳出 IP 位址 {#outbound-ip-addresses}

傳出連線是 Marketo Engage 代表您與網際網路上的伺服器所建立的連線。與您合作的部分合作夥伴/廠商或者您自己的 IT 組織可能會使用允許清單來限制對伺服器的存取。如果是這樣，您必須把 Marketo Engage 的傳出 IP 位址區塊提供給他們，以便新增至允許清單中。

**Webhook**

Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} 為傳出整合機制。在智慧行銷活動中，執行[呼叫 Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} 流程動作時，會向外部 Web 服務發出 HTTP 要求。如果 Web 服務發佈者使用外部 Web 服務所在網路的防火牆上的允許清單，則發佈者必須將下列 IP 位址區塊新增至其允許清單。

**CRM 同步**

Marketo Engage [Salesforce CRM Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} 和 [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} 為整合機制，會向您的 CRM 廠商所發佈的 API 發送傳出 HTTP 要求。您必須確保您的 IT 組織不會封鎖下列任何 IP 位址區塊，而使其無法存取您的 CRM 廠商 API。

**Marketo Engage 傳出 IP 位址區塊**

下列表格會涵蓋所有發出傳出呼叫的 Marketo Engage 伺服器。如果您正在設定任何 IP 允許清單、伺服器、防火牆、存取控制清單、安全性群組或第三方服務來接收來自 Marketo Engage 的傳出連線，請使用以下清單。

<table>
 <tbody>
  <tr>
   <th>IP 區塊 (CIDR 標記法)</th>
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
   <th>個人 IP 地址</th>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
  <tr>
   <td>35.165.244.220</td>
  </tr>
  <tr>
   <td>44.235.171.179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
  <tr>
   <td>54.220.138.65</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
