---
unique-page-id: 2949469
description: 設定步驟 — Marketo文檔 — 產品文檔
title: 設定步驟
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
source-git-commit: 74da8ebbd564b11e2795da31321ca47493135f48
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 0%

---

# 設定步驟 {#setup-steps}

**歡迎來Marketo Engage!**

在開始使用Marketo之前，您需要完成幾個步驟。

這些步驟包括：

* 某些基本帳戶設定
* 將登錄頁URL和電子郵件連結貼上品牌以提高信任度和可交付性
* 正在同步您的CRM
* 向公司網站添加跟蹤代碼

>[!NOTE]
>
>您只需在公司 **新Marketo**。 否則，可能已完成安裝。

某些步驟需要您的IT團隊提供幫助。

>[!TIP]
>
>如果 [打印出核對表](/help/marketo/getting-started/setup/setup-checklist.md){target="_blank"}，可在完成項目時將其檢出。

## 登錄並建立其他Marketo用戶 {#log-in-and-create-additional-marketo-users}

登錄Marketo [這裡](https://app.marketo.com/){target="_blank"} 使用您通過電子郵件收到的憑據。

![](assets/setup-steps-1.png)

恭喜！你現在在Marketo，可以開始探索了。 您可能希望邀請營銷團隊中的同事加入您。 您可以通過添加新用戶來執行此操作。

轉到 **[!UICONTROL 管理]** 的子菜單。

>[!TIP]
>
>在此時，您可以按一下 **[!UICONTROL 我的帳戶]** 更改帳戶和位置設定，並設定新訂閱名稱。

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**需要管理權限**

按一下 **[!UICONTROL 用戶和角色]**。

![](assets/setup-steps-3.png)

按一下 **[!UICONTROL 邀請新用戶]**。

![](assets/setup-steps-4.png)

填寫您同事的電子郵件地址、名字和姓氏。 _設定訪問到期日期是可選的_。 按一下 **[!UICONTROL 下一個]**。

![](assets/setup-steps-5.png)

>[!TIP]
>
>到期日對短期外部利益攸關者或顧問來說非常合適，他們只需在短期內訪問Marketo。

>[!NOTE]
>
>到期日期到達時，用戶收到到期通知，帳戶被鎖定。

選擇角色並按一下 **[!UICONTROL 下一個]**。 標準用戶有權訪問除管理員之外的所有區域。

![](assets/setup-steps-6.png)

>[!NOTE]
>
>除了五個內置角色之外，您還可以建立自定義角色。 瞭解有關 [管理用戶角色和權限](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}。

請隨意修改邀請文本。 按一下 **發送**。

![](assets/setup-steps-7.png)

新用戶現在列在 **[!UICONTROL 用戶]** 頁籤，並應接收包含建立密碼和登錄的連結的電子郵件。 下一步！

![](assets/setup-steps-8.png)

## 設定授權支援聯繫人 {#set-up-your-authorized-support-contacts}

您可能收到了一封來自Marketo支援的電子郵件，聲明您是您公司的Marketo客戶支援管理員。 如果是，您可以設定 **授權支援聯繫人** 為你的團隊。 只有授權的支援聯繫人才能通過以下方式直接與Marketo客戶支援聯繫： [Marketo支援門戶](https://support.marketo.com){target="_blank"}。

>[!NOTE]
>
>您可以建立的支援聯繫人數量由您購買的包決定。 此限制在您從Marketo支援部門發來的電子郵件中指定。

授權支援聯繫人文檔已移至Marketo社區。 請參閱 [這篇文章](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}。

>[!NOTE]
>
>只有登錄到Marketo社區的人才出現在清單中。 如果找不到此人，請確保他們首先登錄到社區。

## 使用CNAME自定義登錄頁URL {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 可以跳過此步驟。 在啟動呼叫期間，顧問將為您提供IT設定說明文檔。

>[!NOTE]
>
>**需要管理權限**

為登錄頁選擇CNAME。 一些示例：

    **去**。[CompanyDomain].com
    **www2**。[CompanyDomain].com
    * **lp**。[CompanyDomain].com

>[!TIP]
>
>保持短！ 更短的URL更容易記住。 我們建議把&quot;go&quot;作為域。

第一部分（粗體）是 `[LandingPageCNAME]`。 在步驟5中，您需要它。

要檢索要用登錄頁CNAME替換的Munchkin ID，請轉到「管理」區域。

![](assets/setup-steps-9.png)

按一下 **我的帳戶**。

![](assets/setup-steps-10.png)

複製 [!UICONTROL 帳戶字串] 從登錄頁設定。

![](assets/setup-steps-11.png)

這是 `[Munchkin ID]`。 保存它。 您需要在步驟5中將其交給IT部門。

配置域設定，以便登錄頁使用您公司的域，而不是Marketo的域（它們的托管地）。

## 確保電子郵件傳輸能力 {#ensure-email-deliverability}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 可以跳過此步驟。 在啟動呼叫期間，顧問將為您提供IT設定說明文檔。

您可以採取多種措施來確保電子郵件能夠覆蓋盡可能多的人。

* **標籤跟蹤連結**。 您可以選擇一個CNAME，以在您從Marketo發來的電子郵件中包含的連結中使用您自己的域(而不是Marketo的域)。 這增強了您的域品牌推廣能力，並提高了與收件人的信任和交付能力。
* **將Marketo添加到您的公司電子郵件允許清單中。** 在向實際人員發送電子郵件之前，將test電子郵件發送到test帳戶是一種常見的最佳做法。 通過允許Marketo，您可以防止這些test電子郵件被阻止或標籤為垃圾郵件。
* **設定SPF和DKIM。** 這些技術可確保您的收件人確信您的Marketo電子郵件不是垃圾郵件。 要幫助防止收件人的垃圾郵件過濾器拒絕您的Marketo電子郵件，請執行以下步驟： [設定電子郵件傳送功能的SPF和DKIM](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md)。
* **為域設定MX記錄。** MX記錄允許您將郵件接收到要發送電子郵件的域，以處理回復和自動應答器。 如果您正從公司域發送，則可能已配置了此功能。 否則，通常可以設定為映射到公司域的MX記錄。
* **建議的「發件人地址」設定。** 您必須在所有電子郵件市場活動的「發件人地址」中使用有效、現有且有效的電子郵件域。 配置公司域的子域而不是從公司域發送可能會有所幫助。 這將確保公司郵件流中的問題不會影響您的Marketo郵件流，反之亦然。 此外，從 `something@nonexistentdomain.com` 將導致電子郵件被過濾或阻止。 發件人的「發件人地址」中使用的任何域都必須具有有效且工作的postmaster@和uspase@帳戶。

如果您正在使用Google應用程式托管您的公司電子郵件，您將無法在您的域下建立「濫用」@或「郵件管理員」@電子郵件。 要繞過這一點，您需要建立名為「濫用」和「郵政管理員」的組。 屬於這些組的用戶將收到發送到這些地址(例如postmaster@domain.com)的電子郵件。 有關建立組的詳細說明 [這裡](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}。

為電子郵件跟蹤連結選擇CNAME(選擇一個 _不同_ 在步驟3中選擇的登錄頁CNAME中。 一些示例：

* go2。[公司域].com
* 埃姆。[公司域].com
* 哇。[公司域].com

第一部分是電子郵件跟蹤CNAME `[EmailTrackingCNAME]`。 您需要在步驟5中將其交給IT部門。

>[!CAUTION]
>
>電子郵件和登錄頁CNAME必須不同。 另外，避免像「track」或「link」這樣的CNAME。 它通常被標籤為垃圾郵件

要查找您的Marketo跟蹤連結，請轉到 **[!UICONTROL 管理]** 的子菜單。

![](assets/setup-steps-12.png)

按一下 **[!UICONTROL 電子郵件]**。

![](assets/setup-steps-13.png)

複製 [!UICONTROL 跟蹤連結] 從您的電子郵件設定中。

的 [!UICONTROL 跟蹤連結] 為： `mkto-[a-z][4 digits].com`。

![](assets/setup-steps-14.png)

這是你的 `[MktoTrackingLink]`。 保存它。 您需要在步驟5中將其交給IT部門。

收集「發件人」域。 列出所有「發件人」域（如中所示） `[Sender]@[FromDomain].com`)，您計畫用於發送Marketo的電子郵件。 對大多數人來說，只有一個。

例如，&#39;marketo.com&#39;, &#39;info.marketo.com&#39;。 這些 `[FromDomain1]`。`[FromDomain2]`的子菜單。 救他們。 您需要在步驟5中將它們交給IT部門。

您現在擁有將請求發送到IT所需的所有資訊！

## 請IT人員配置協定 {#ask-it-to-configure-protocols}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 可以跳過此步驟。 在啟動呼叫期間，顧問將為您提供IT設定說明文檔。

一旦收集了所有必要的資訊，您就可以向IT部門發送請求。 您可以將下面的文本用作模板，用您自己的資訊替換粗體文本。

[包括指向此文章的連結](/help/marketo/getting-started/setup/configure-protocols-for-marketo.md)。

將此文本貼上到電子郵件中，並替換帶粗體的佔位符：

>[!NOTE]
>
>請參閱上面的步驟3和4以確定替換佔位符的文本。 記住 `[LandingPageCNAME]` 和 `[EmailTrackingCNAME]` 一定不一樣。

`----------------------------------------------`

尊敬的IT管理員：

我們的營銷團隊現在正在使用Marketo平台與我們的人員溝通。 為確保電子郵件傳輸效能優異，我們需要進行以下更改：

`1)` 對於登錄頁，添加DNS條目(CNAME) **[登錄頁名稱]**。**[公司域]**.com，指向 **[蒙奇金ID]**.mktoweb.com。

`2)` 對於電子郵件中的跟蹤連結，請為 **[電子郵件跟蹤CNAME]**。**[公司域]**.com，指向 **[MktoTrackingLink]**。

`3)` 允許Marketo。

    *如果我們在「電子郵件允許清單」中使用IP地址，請添加下面列出的IP:
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    94.236.119.0/26

>[!NOTE]
>
>如果您希望IP的縮寫清單允許您的環境特定清單，請聯繫Marketo支援。

    *如果我們的反垃圾郵件系統使用「發件人」域，請添加以下內容：

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` 我們需要設定SPF和DKIM，以便Marketo有權代表我們發送簽名的電子郵件。

`a.` 要設定SPF，請將以下行添加到我們的DNS條目：

IN TXT **[從域]**:v=spf1 mx ip4:**[公司IP]**
<br/>包括：mtomail.com ~all

如果我們的DNS條目中已有SPF記錄，只需將以下內容添加到該條目：

包括：mktomail.com

`[`替換 **從域** 域中的電子郵件(例如：company.com和 **公司IP** 公司電子郵件伺服器的IP地址(例如：255.255.255.255)。  如果您要通過Marketo從多個域發送電子郵件，您應讓您的IT人員為每個域（在一行上）添加此行。`]`

`b.` 對於DKIM，請為要設定的每個域建立DNS資源記錄。 下面是我們將為其簽名的每個域的主機記錄和TXT值：

**`[DKIMDomain1]`**:主機記錄為 **`[HostRecord1]`** TXT值為 **[TXTValue1]**。

**`[DKIMDomain2]`**:主機記錄為 **`[HostRecord2]`** TXT值為 **`[TXTValue2]`**。

`[`複製 **主機記錄** 和 **TXTValue** 每 **基姆多曼** 您在 [說明](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)。 不要忘記驗證中的每個域 **管理員>電子郵件> DKIM** 在您的IT員工完成此步驟後。`]`

`5)` 我們需要確保我們的FROM域有有效的MX記錄 **[源域1]**。 **[源域2]**&#x200B;的子菜單。 你能證實嗎？ 否則，請配置為映射到公司域MX記錄。 這將確保我們能夠處理對Marketo郵件的答復/自動應答器。

在您完成這些步驟後，請通知我，以便我可以完成與Marketo的設定過程。

謝謝！ 你是最棒的！

愛，

**`[Your Name]`**

`----------------------------------------------`

向IT部門發送電子郵件。 我們知道， IT可能需要一些時間來完成這些任務。 您可以繼續執行步驟7，但請記住必須返回步驟6才能完成Marketo設定。

## 在IT完成後完成Marketo設定 {#complete-your-marketo-setup-after-it-finishes}

IT人員完成任務後，請按照以下步驟添加登錄頁和電子郵件CNAME，並激活DKIM簽名。

轉到 **[!UICONTROL 管理]** 添加登錄頁CNAME的區域

![](assets/setup-steps-15.png)

選擇登錄頁並按一下 **[!UICONTROL 編輯]** 的 [!UICONTROL 設定] 的子菜單。

![](assets/setup-steps-16.png)

在欄位中輸入新域名 **[!UICONTROL 登錄頁的域名]**。 這應該是：

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

在 **[!UICONTROL 回退]** 頁面，輸入在登錄頁不可用時希望人們轉到的URL。 如果沒有備用頁，則可以使用公司首頁。 在 **[!UICONTROL 首頁]** 欄位，輸入公司網站。

![](assets/setup-steps-18.png)

在 [!UICONTROL 管理] ，選擇 **[!UICONTROL 電子郵件]** 添加電子郵件CNAME

![](assets/setup-steps-19.png)

向下滾動到 [!UICONTROL 品牌域]。 選擇域並按一下 **[!UICONTROL 編輯]**。

![](assets/setup-steps-20.png)

在「域」欄位中，輸入電子郵件跟蹤域。 這應該是：

`[EmailTrackingCNAME].[CompanyDomain].com`. 按一下 **[!UICONTROL 保存]**。

![](assets/setup-steps-21.png)

## 整合您的CRM {#integrate-your-crm}

這可能是您設定過程中最激動人心的一步 — 是時候讓Marketo滿足您儲存在CRM中的所有這些線索和聯繫人了！

根據您公司使用的CRM，從以下選項中進行選擇。

    * [將Marketo與 [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [將Marketo與 [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>您需要公司CRM管理員的幫助才能完成這些步驟。

## 將跟蹤代碼添加到您的網站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>你是 [!DNL Launch Pack] 客戶？ 可以跳過此步驟。 您的顧問將為您提供 [!DNL Munchkin] IT設定說明文檔中的代碼說明。

Marketo有自定義跟蹤JavaScript(稱為 [!DNL Munchkin])，用於跟蹤任何網頁上的人員活動。 [!DNL Munchkin] 需要將您的網站整合到Marketo。 按照以下步驟執行 [添加 [!DNL Munchkin] 跟蹤網站代碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}。

>[!NOTE]
>
>添加跟蹤代碼所需的HTML體驗。

## 效能期望 {#performance-expectations}

你對Marketo的表現能期待多少？ 根據您的營銷活動的規模和複雜性，它可能會有所不同。 但是，您可以期望效能級別與「標準」列中概述的效能級別相同，該列位於 [Marketo Engage產品說明](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. The "Performance" and "Performance Plus" columns refer to performance tier packages that provide [higher performance levels](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}。

所有設定步驟都結束。 剩下的就是潛進去，用Marketo!
