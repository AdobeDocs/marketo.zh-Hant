---
unique-page-id: 4720433
description: 設定Marketo的通訊協定 — Marketo檔案 — 產品檔案
title: 設定Marketo的通訊協定
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 2c293eacb0dd693118efc0260118337eb671c1b9
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 2%

---

# 設定Marketo的通訊協定 {#configure-protocols-for-marketo}

如果您或您的組織使用限制性的防火牆或Proxy伺服器設定，您或您的網路管理員可能需要將某些網域和IP位址範圍列入允許清單，以確保Adobe Marketo Engage如期運作。

如需協助實作下列通訊協定，請與您的IT部門分享本文章。 如果他們使用允許清單來限制Web存取，請確定他們新增以下網域（包括星號），以允許所有Marketo資源和網站通訊端：

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## 步驟1：建立登入頁面和電子郵件的DNS記錄 {#step-create-dns-records-for-landing-pages-and-email}

**追蹤連結CNAME**

您的行銷團隊應傳送兩則新CNAME記錄的要求給您。 第一個是用於登入頁面URL，讓登入頁面以可反映您網域的URL顯示，而非以Marketo （實際主機）顯示。 第二個用於追蹤從Marketo傳送之電子郵件中所包含的連結。

`1` **為登陸頁面新增CNAME**

將他們傳送給您的登陸頁面CNAME新增至您的DNS記錄，以便 `[YourLandingPageCNAME]` 指向指派給您Marketo登陸頁面的唯一帳戶字串。 登入您的網域註冊機構的網站，然後輸入登陸頁面CNAME和帳戶字串。 這通常涉及三個欄位：

* 別名：輸入 `[YourLandingPageCNAME]` （行銷提供）
* 型別： CNAME
* 指向：輸入 `[MunchkinID].mktoweb.com` （行銷提供）

`2` **為電子郵件追蹤連結新增CNAME**

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

## 步驟2：將Marketo IP加入允許清單 {#step-allowlist-marketo-ips}

當您的行銷群組使用Marketo傳送測試電子郵件（在傳送電子郵件爆炸前的最佳實務）時，測試電子郵件有時會被反垃圾郵件系統封鎖，這些系統依賴寄件者IP位址來驗證電子郵件是否有效。 為確保這些測試電子郵件送達，請將Marketo新增至您的允許清單。

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

有些反垃圾郵件系統使用電子郵件傳迴路徑欄位而不是允許的IP位址。 在這些情況下，最好的辦法是加入允許清單&#39;&#42;.mktomail.com&#39;，因為Marketo使用數個信箱子網域。 其他反垃圾郵件系統根據寄件者地址加入允許清單。 在這些情況下，請務必加入您的行銷群組用來與人員/潛在客戶通訊的所有傳送（「寄件者」）網域。

>[!NOTE]
>
>Postini採用獨特的技術，並需要將IP範圍列入允許清單。 另請參閱 [使用Postini加入允許清單](https://nation.marketo.com/docs/DOC-1066).

## 步驟3：設定SPF和DKIM {#step-set-up-spf-and-dkim}

您的行銷團隊也應傳送要新增至DNS資源記錄（亦列於下方）的DKIM （網域金鑰識別郵件）資訊給您。 按照步驟成功設定DKIM和SPF (Sender Policy Framework)，然後通知您的行銷團隊這已更新。

1. 若要設定SPF，請在我們的DNS專案中新增下列行：

   `[CompanyDomain]` 在TXT中v=spf1 mx ip4：`[CorpIP]`\
   包含： mktomail.com ~all

   如果我們的DNS專案中已有現有的SPF記錄，只需新增下列內容即可：\
   包含： mktomail.com

   將CompanyDomain取代為您網站的主網域(例如： 」`(company.com/)`&quot;)和CorpIP，以及您企業電子郵件伺服器的IP位址(例如 &quot;255.255.255.255&quot;). 如果您要透過Marketo從多個網域傳送電子郵件，請讓IT人員為每個網域新增此行（在同一行）。

1. 針對DKIM，請為每個要設定的網域建立DNS資源記錄。 我們將簽署的每個網域的主機記錄和TXT值如下：

   `[DKIMDomain1]`：主機記錄為 `[HostRecord1]` 且TXT值為 `[TXTValue1]`.

   `[DKIMDomain2]`：主機記錄為 `[HostRecord2]` 且TXT值為 `[TXTValue2]`.

   在遵循下列步驟之後，針對您設定的每個DKIMDomain複製HostRecord和TXTValue [此處提供指示](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. IT人員完成此步驟後，別忘了在「管理員>電子郵件> DKIM」中驗證每個網域。

## 步驟4：設定DMARC {#set-up-dmarc}

DMARC （網域型訊息驗證、報告及一致性）是一種驗證通訊協定，用於協助組織保護其網域免受未經授權的使用。 DMARC會擴充現有的驗證通訊協定（例如SPF和DKIM），以通知收件者伺服器如果網域發生驗證失敗時應採取的動作。 雖然DMARC目前是選用專案，但強烈建議您使用，因為這樣可以更好地保護組織的品牌和聲譽。 自2024年2月起，Google和Yahoo等主要提供者將要求為大量傳送者使用DMARC。

若要讓DMARC運作，您必須至少擁有下列其中一個DNS TXT記錄：

* 有效的SPF
* 您的FROM：網域的有效DKIM記錄(建議用於Marketo Engage)

此外，您必須擁有您的FROM：網域的DMARC特定DNS TXT記錄。 您可選擇定義您選擇的電子郵件地址，指出DMARC報告應在組織內的哪個位置，以便您監視報告。

作為最佳實務，建議您逐步推出DMARC實作，將DMARC政策從p=none提升至p=quarantine、再提升至p=reject，因為您可以瞭解DMARC的潛在影響，並將DMARC政策設定為在SPF和DKIM上輕鬆保持一致。

### DMARC範例工作流程 {#dmarc-example-workflow}

1. 如果您已設定為可接收DMARC報告，您應該執行下列動作……

   I.分析您收到並使用的意見與報告(p=none)，告知接收者不對驗證失敗的郵件執行任何動作，但仍會傳送電子郵件報告給寄件者。

   二、 如果合法的訊息驗證失敗，請檢閱並修正SPF/DKIM的問題。

   三、 判斷SPF或DKIM是否已對齊，並傳遞所有合法電子郵件的驗證。

   四、 請檢閱報告，以確保根據SPF/DKIM政策得出的結果符合您的預期。

1. 繼續將原則調整為(p=quarantine)，這會通知接收電子郵件伺服器隔離驗證失敗的電子郵件（這通常表示將這些郵件放在垃圾郵件資料夾中）。

   I.檢閱報表，確保結果如您預期般如實。

1. 如果您對p=隔離層級的訊息行為感到滿意，您可以將原則調整為（p=拒絕）。 p=reject原則會告訴接收者，對於驗證失敗的網域，要完全拒絕（退回）任何電子郵件。 啟用此原則後，只有經過網域驗證為100%驗證的電子郵件才有機會放置收件匣。

>[!CAUTION]
>
>請謹慎使用此原則，並判斷其是否適合您的組織。

### DMARC報告 {#dmarc-reporting}

DMARC提供接收有關未通過SPF/DKIM之電子郵件的報表的功能。 在驗證流程中，ISP服務程式會產生兩個不同的報告，讓傳送者可透過其DMARC原則中的RUA/RUF標籤接收。

* 彙總報表(RUA)：不包含任何會對GDPR （一般資料保護規範）敏感的PII （個人識別資訊）。

* 鑑證報告(RUF)：包含對GDPR敏感的電子郵件地址。 在使用之前，最好從內部檢查如何處理需要符合GDPR的資訊。

這些報告的主要用途是接收企圖詐騙的電子郵件概觀。 這些是高度技術性的報告，最好透過協力廠商工具消化。

### 範例DMARC記錄 {#example-dmarc-records}

* 裸機最小記錄： `v=DMARC1; p=none`

* 記錄指向接收報告的電子郵件地址： `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### DMARC標籤及其功用 {#dmarc-tags-and-what-they-do}

DMARC記錄有多個稱為DMARC標籤的元件。 每個標籤都有一個值，指定DMARC的特定外觀。

<table>
<thead>
  <tr>
    <th>標籤名稱 </th>
    <th>必要/選用 </th>
    <th>函數 </th>
    <th>範例 </th>
    <th>預設值 </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>必要</td>
    <td>此DMARC標籤指定版本。 目前只有一個版本，因此其固定值為v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>必要</td>
    <td>顯示選取的DMARC原則，並指示接收者報告、隔離或拒絕驗證檢查失敗的郵件。</td>
    <td>p=none、quarantine或reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>可選</td>
    <td>允許網域擁有者指定報告選項。</td>
    <td>0：如果一切失敗，則產生報表 
    <br>1：發生任何失敗時產生報表 
    <br>d：如果DKIM失敗則產生報告 
    <br>s：如果SPF失敗，則產生報表</td>
    <td>1 （建議用於DMARC報表）</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>可選</td>
    <td>告知受篩選的訊息百分比。</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>規則</td>
    <td>選用（建議）</td>
    <td>識別彙總報表的傳送位置。</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>選用（建議）</td>
    <td>識別將傳送鑑證報告的位置。</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>可選</td>
    <td>指定上層網域之子網域的DMARC原則。</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>可選</td>
    <td>可以是「嚴格」(Strict) (s)或「寬鬆」®數。 寬鬆的對齊表示DKIM簽章中使用的網域可以是「寄件者」位址的子網域。 嚴格對齊表示DKIM簽章中使用的網域必須與寄件者位址中使用的網域完全相符。</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>可選</td>
    <td>可以是「嚴格」(Strict) (s)或「寬鬆」®數。 寬鬆的對齊表示ReturnPath網域可以是「寄件者地址」的子網域。 嚴格對齊表示傳迴路徑網域必須與寄件者位址完全相符。</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

如需DMARC及其所有選項的完整詳細資訊，請造訪 [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC與Marketo Engage {#dmarc-and-marketo-engage}

DMARC有兩種對齊方式：DKIM對齊方式和SPF對齊方式。

>[!NOTE]
>
>建議在Marketo的DKIM與SPF上執行DMARC對齊。

* DKIM-aligned DMARC — 若要設定DKIM-aligned DMARC，您必須：

   * 為訊息的FROM：網域設定DKIM。 使用指示 [本文章](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * 為先前設定的FROM：/DKIM網域設定DMARC

* DMARC-aligned SPF — 若要透過品牌傳迴路徑設定DMARC-aligned SPF，您必須：

   * 設定品牌化傳迴路徑網域
      * 設定適當的SPF記錄
      * 變更MX記錄，以指向將傳送郵件之資料中心的預設MX

   * 為品牌傳迴路徑網域設定DMARC

* 如果您是透過專用IP從Marketo傳送郵件，但尚未實作品牌傳迴路徑，或不確定您是否有，請開啟票證並附上 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* 如果您透過共用IP集區從Marketo傳送郵件，您可以透過以下方式檢視您是否符合信任的IP資格 [在此套用](http://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. 品牌傳迴路徑免費提供給從Marketo信任的IP傳送的訪客。 如果核准此計畫，請聯絡Marketo支援以設定品牌傳迴路徑。

   * 信任的IP：為每月傳送不到75K且不符合專用IP資格之較低磁碟區使用者的共用IP集區。 這些使用者也必須符合最佳實務需求。

* 如果您是透過共用IP從Marketo傳送郵件，但您不符合信任的IP資格，且每月傳送的郵件超過100,000封，您將需要聯絡Adobe帳戶團隊（您的帳戶經理）以購買專用IP。

* Marketo中不支援也不建議使用嚴格SPF對齊。

## 步驟5：為您的網域設定MX記錄 {#step-set-up-mx-records-for-your-domain}

MX記錄可讓您接收寄送電子郵件至之網域的郵件，以處理回覆和自動回應者。 如果您要從公司網域傳送，您可能已經設定好此專案。 如果沒有，您通常可以將其設定為對應到您公司網域的MX記錄。

## 傳出IP位址 {#outbound-ip-addresses}

輸出連線是指Marketo Engage代表您連線至網際網路上的伺服器。 與您合作或您自己的IT組織的一些合作夥伴/廠商可能會使用允許清單來限制對伺服器的存取。 若是如此，您必須提供Marketo Engage的輸出IP位址區塊，以新增至其允許清單。

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} 流程動作是在智慧行銷活動中執行，會向外部Web服務發出HTTP請求。 如果Web服務發佈者使用外部Web服務所在網路的防火牆上的允許清單，則發佈者必須將下列的IP位址區塊新增至其允許清單。

**CRM同步**

Marketo Engage [Salesforce CRM同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} 是整合機制，可向您的CRM供應商發佈的API發出傳出HTTP請求。 您必須確保您的IT組織不會封鎖下列任何IP位址區塊，使其無法存取您的CRM供應商API。

**Marketo Engage傳出IP位址區塊**

下表涵蓋進行傳出呼叫的所有Marketo Engage伺服器。 如果您要將任何IP允許清單、伺服器、防火牆、存取控制清單、安全性群組或協力廠商服務設定為接收來自Marketo Engage的傳出連線，請使用下列清單。

<table>
 <tbody>
  <tr>
   <th>IP區塊（CIDR標籤法）</th>
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
   <th>個別IP位址</th>
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
  </tr>
   <tr>
   <td>130.248.168.16</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
 </tbody>
</table>
