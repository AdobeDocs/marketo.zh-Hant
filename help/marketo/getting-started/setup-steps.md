---
unique-page-id: 2949469
description: 設定步驟——行銷人員檔案——產品檔案
title: 設定步驟
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '2004'
ht-degree: 0%

---


# 設定步驟{#setup-steps}

**馬克托歡迎你！**

在您投入使用Marketo之前，您需要先完成幾個步驟。

這些步驟包括：

* 基本帳戶設定
* 將登陸頁面URL和電子郵件連結品牌化，以提升信任度和傳遞能力
* 同步您的CRM
* 新增追蹤代碼至公司網站

>[!NOTE]
>
>如果您的公司是&#x200B;**新進行Marketo**，則只需執行這些步驟。 否則，可能已完成設定。

有些步驟需要IT團隊的協助。

>[!TIP]
>
>如果您[列印出此檢查清單](/help/marketo/getting-started/setup-steps/setup-checklist.md)，您可以在完成項目時將項目勾選。

## 登入並建立其他Marketo使用者{#log-in-and-create-additional-marketo-users}

1. 使用您透過電子郵件收到的認證登入Marketo [here](https://app.marketo.com/)。

   ![](assets/new-login-screen-hand.jpg)

恭喜！ 您現在已進入Marketo，可以開始探索。 您可能會想邀請行銷團隊的同事加入您。 您可以新增使用者來完成此作業。

前往&#x200B;**Admin**&#x200B;區域。

>[!TIP]
>
>在此期間，您可以按一下「我的帳戶」**以變更您的帳戶和位置設定，並設定新的訂閱名稱。**

![](assets/admin.png)

>[!NOTE]
>
>**需要管理員權限**

按一下「**用戶和角色**」。

![](assets/image2015-1-6-13-3a14-3a43.png)

按一下「邀請新使用者」。****

![](assets/image2015-1-6-13-3a14-3a6.png)

填寫您同事的電子郵件地址、名字和姓氏。

![](assets/image2016-5-24-10-3a11-3a12.png)

（可選）使用日曆選擇器輸入邀請的原因和訪問到期日。 按一下&#x200B;**確定**。

![](assets/image2016-5-24-10-3a13-3a9.png)

按一下&#x200B;**Next**。

![](assets/image2016-5-24-10-3a14-3a9.png)

>[!TIP]
>
>到期日對短期外部利益相關者或顧問非常適合，他們只需要Market才能短暫存取。

>[!NOTE]
>
>到期日到來時，使用者會收到到期通知，而帳戶會被鎖定。

選擇角色並按一下&#x200B;**Next**。 「標準使用者」可存取除「管理員」以外的所有區域。

![](assets/image2016-5-24-10-3a14-3a51.png)

>[!NOTE]
>
>除了5個內建角色外，您也可以建立自訂角色。 進一步瞭解[管理使用者角色和權限](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)。

您可以隨意調整邀請文字。 按一下&#x200B;**發送**。

![](assets/image2016-5-24-10-3a15-3a52.png)

現在，新使用者會列在「使用者」索引標籤中，而且應該會收到含有建立密碼和登入連結的電子郵件。 下一步！

![](assets/image2016-5-24-10-3a23-3a10.png)

## 設定您的授權支援聯繫人{#set-up-your-authorized-support-contacts}

您可能已收到Marketo Support寄來的電子郵件，指出您是貴公司的Marketo Customer Support管理員。 如果是，您可以為團隊設定&#x200B;**授權支援聯繫人**。 只有授權的支援聯絡人才能直接透過[行銷支援入口網站](https://support.marketo.com)與行銷客戶支援聯絡。

>[!NOTE]
>
>您可以建立的支援連絡人數，由您購買的套件決定。 此限制是在您從行銷人員寄至支援的電子郵件中指定。

授權支援連絡檔案已移至Marketo社群。 請參閱[本文](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341)。

>[!NOTE]
>
>只有登入Marketo社群的人員才會出現在清單中。 如果您找不到該人，請確定他們先登入社群。

## 使用CNAME {#customize-your-landing-page-urls-with-a-cname}自訂著陸頁面URL

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您的啟動通話期間提供IT設定指示檔案。

>[!NOTE]
>
>**需要管理員權限**

為您的登陸頁面選擇CNAME。 例如：

    * **go**。[CompanyDomain].com
    * **www2**。[CompanyDomain].com
    * **lp**。[CompanyDomain].com

>[!TIP]
>
>小點！ 較短的URL更容易記住。 我們建議把&quot;go&quot;當成網域。

第一部分（粗體）是`[LandingPageCNAME]`。 在步驟5中，您將需要它。

若要擷取將要取代為著陸頁面CNAME的帳戶字串，請前往「管理員」區域。

![](assets/admin.png)

按一下「著陸頁面&#x200B;**」。**

![](assets/image2015-1-6-13-3a52-3a6.png)

從登陸頁面設定複製帳戶字串。

![](assets/image2015-1-6-13-3a53-3a19.png)

這是`[AccountString]`。 保存。 您需要在步驟5中將它提供給IT部門。

設定您的網域設定，讓登陸頁面使用您公司的網域，而非Marketo的網域（其所在位置）。

## 確保電子郵件傳遞能力{#ensure-email-deliverability}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您的啟動通話期間提供IT設定指示檔案。

您可以採取數種措施來確保電子郵件能觸及到盡可能多的人。

    1.**品牌化您的追蹤連結**。 您可以選擇CNAME，在您從Marketo寄送的電子郵件中所包含的連結中，使用您自己的網域（而非Marketo）。 這可強化您的網域品牌，並提高您與收件者的信任和傳遞能力。
    1.**將Marketo新增至您的公司電子郵件允許清單。**在傳送電子郵件給實際使用者之前，先將測試電子郵件傳送至您的測試帳戶是常見的最佳做法。 借由允許Marketto，您可以防止這些測試電子郵件遭到封鎖或標幟為垃圾訊息。
    1.**設定SPF和DKIM。**這些技術可確保您的收件者確信您的行銷人員電子郵件並非垃圾郵件。 為協助防止收件者的垃圾訊息篩選器拒絕您的Marketo電子郵件，請依照下列步驟執行[設定SPF和DKIM以取得您的電子郵件傳送能力](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md)。
    1.**為您的網域設定MX記錄。** MX記錄可讓您接收寄送電子郵件至網域的郵件，以處理回覆和自動回覆者。 如果您是從公司網域傳送，則可能已設定此設定。 若未設定，您通常可設定為對應至您公司網域的MX記錄。
    1.**建議的起始位址設定。**您必須在所有電子郵件促銷活動的「寄件者位址」中使用有效、現有且有效的電子郵件網域。 設定公司網域的子網域，而非從公司網域傳送，可能會有好處。 如此可確保您公司mailstream的問題不會影響您的Marketo mailstream，反之亦然。 此外，從something@nonexistentdomain.com傳送郵件會導致篩選或封鎖電子郵件。 發件人地址中使用的任何域都必須具有有效且有效的postmaster@和upuse@帳戶。
    如果您使用Google Apps代管公司電子郵件，將無法在您的網域下建立ubuse@或postmaster@電子郵件。為瞭解決這個問題，您需要建立名為「濫用」和「郵遞員」的組。 屬於這些群組成員的使用者將會收到傳送至這些位址的電子郵件(例如postmaster@domain.com)。 有關建立群組的詳細說明，請參閱[此處](https://support.google.com/a/answer/33343#adminconsole)。

選擇電子郵件追蹤連結的CNAME（從您在步驟3中選擇的著陸頁面CNAME中選擇&#x200B;_different_&#x200B;的CNAME）。 例如：

    * go2。[CompanyDomain].com
    * em。[CompanyDomain].com
    * wow.[CompanyDomain].com

第一部分是電子郵件追蹤CNAME, `[EmailTrackingCNAME]`。 您需要在步驟5中將它提供給IT部門。

>[!CAUTION]
>
>電子郵件和著陸頁面CNAME必須不同。 此外，請避免CNAME（例如「track」或「link」）。 它通常被標幟為垃圾訊息

若要尋找您的行銷人員追蹤連結，請前往&#x200B;**管理員**&#x200B;區域。

![](assets/admin.png)

按一下&#x200B;**電子郵件**。

![](assets/image2015-1-6-13-3a55-3a32.png)

從您的電子郵件設定複製追蹤連結。

「追蹤連結」的格式為：`mkto-[a-z][4 digits].com`。

![](assets/email-tracking-link-hand.jpg)

這是您的`[MktoTrackingLink]`。 保存。 您需要在步驟5中將它提供給IT部門。

收集「來源」網域。 列出您打算用來傳送Marketo電子郵件的所有「寄件者」網域（如中，`[Sender]@[FromDomain].com`）。 對大多數人來說，只有一個。

例如，&#39;marketo.com&#39;、&#39;info.marketo.com&#39;。 這些是`[FromDomain1]`、`[FromDomain2]`等。 儲存它們。 您需要在步驟5中將它們交給IT部門。

您現在擁有將要求傳送給IT人員所需的所有資訊！

## 要求IT人員配置{#ask-it-to-configure-protocols}協定

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您的啟動通話期間提供IT設定指示檔案。

收集完所有必要資訊後，您就可以向IT部門傳送要求。 您可以使用下方的文字做為範本，以您自己的資訊取代粗體文字。

[包含此文章的連結](/help/marketo/getting-started/setup-steps/configure-protocols-for-marketo.md)。

將此文字貼到電子郵件中，並取代粗體預留位置：

>[!NOTE]
>
>請參閱上述步驟3和4，以決定要取代預留位置的文字。 請記住，`[LandingPageCNAME]`和`[EmailTrackingCNAME]`必須不同。

`---------------------------------------------`

親愛的Awesome IT管理員：

我們的行銷團隊現在正使用Marketo平台與我們的人員溝通。 為確保電子郵件的傳遞能力，我們需要進行下列變更：

`1)` 對於我們的著陸頁面，請為 **[LandingPageCNAME新增DNS項目(CNAME)]**。**[CompanyDomain]**.com，指向 **[AccountString]**.mktoweb.com。

`2)` 若是我們的電子郵件追蹤連結，請新增 **[EmailTrackingCNAME的DNS項目(CNAME)]**。**[CompanyDomain]**.com，指向 **[MktoTrackingLink]**。

`3)` 允許Marketto。

    *如果我們在「電子郵件允許清單」中使用IP位址，請新增下列IP:
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    
    
    103.237.104.0/2294.236.119.0/26

注意：如果您想要提供特定於您環境的IP清單，請聯絡行銷支援。

    *如果我們的反垃圾郵件系統使用「發件人」域，請添加以下內容：

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` 我們需要設定SPF和DKIM，才能授權Marketo代表我們傳送已簽署的電子郵件。

`a.` 要設定SPF，請在DNS條目中添加以下行：

IN TXT **[From Domain]**: v=spf1 mx ip4:**[公司IP(s)]**
<br/>包括：mktomail.com ~all

如果我們的DNS條目中已有SPF記錄，只需在其中添加以下內容：

include:mktomail.com

`[`從網 **域** 取代您的電子郵件(例如：company.com)和 **** CorpIP，以及您公司電子郵件伺服器的IP位址(例如：255.255.255.255)。如果您要透過Marketo從多個網域傳送電子郵件，您的IT人員應為每個網域（在一行）新增此行。`]`

`b.` 對於DKIM，請為每個要設定的域建立DNS資源記錄。以下是我們將簽署的每個網域的主機記錄和TXT值：

**`[DKIMDomain1]`**:主機記錄 **`[HostRecord1]`** 為，TXT值為 **[TXTValue1]**。

**`[DKIMDomain2]`**:主機記錄 **`[HostRecord2]`** 為，TXT值為 **`[TXTValue2]`**。

`[`請依照此處 **** 的指示，復 **** 制您所設定的每 **** 個DKIMDomaina的HostRecord和 [TXTValue](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)。在您的IT人員完成此步驟後，請記得確認&#x200B;**管理>電子郵件> DKIM**&#x200B;中的每個域。`]`

`5)` 我們需要確保我們的FROM網域 **[FromDomain1]**、 **[FromDomain2]**.....你能確認一下嗎？ 如果沒有，請設定以對應至我們的公司網域MX記錄。 這將確保我們能夠處理對我們Marketo郵件的回覆／自動回覆者。

請告知我您何時完成這些步驟，以便我能與Marketo一起完成設定程式。

謝謝！ 你是最棒的！

愛，

**`[Your Name]`**

`---------------------------------------------`

將電子郵件傳送給IT人員。 我們瞭解IT部門完成這些任務可能需要一些時間。 您可以繼續執行步驟7，但請記住，您必須退回步驟6，才能完成行銷人員設定。

## 在IT完成{#complete-your-marketo-setup-after-it-finishes}後完成行銷設定

IT人員完成工作後，請依照下列步驟新增您的登陸頁面和電子郵件CNAME，並啟動DKIM簽署。

前往&#x200B;**Admin**&#x200B;區域以新增著陸頁面CNAME

![](assets/admin.png)

選擇「著陸頁面」，然後按一下「設定」區域中的「編輯」。****

![](assets/image2015-1-6-13-3a59-3a15.png)

在「著陸頁面的網域名稱」欄位中輸入您的新網域名稱。 這應該是：

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/image2015-1-6-14-3a3-3a6.png)

在「備援頁面」欄位中，輸入當著陸頁面無法使用時，您希望訪客前往的URL。 如果您沒有備援頁面，則可使用您的公司首頁。 在「首頁」欄位中，輸入您的公司網站。

![](assets/image2015-1-6-14-3a2-3a46.png)

在「管理員」區域中，選取「電子郵件」以新增您的電子郵件CNAME

![](assets/image2015-1-6-14-3a5-3a3.png)

向下捲動並按一下「編輯」。****

![](assets/edit-branding-domain.png)

在「網域」欄位中，輸入您的電子郵件追蹤網域。 這應該是：

`[EmailTrackingCNAME].[CompanyDomain].com`.按一下&#x200B;**保存**。

![](assets/new-branding-domain-9-1.png)

## 整合您的CRM {#integrate-your-crm}

這可能是您設定中最令人興奮的步驟——是時候讓Market充實您儲存在CRM中的所有潛在客戶和連絡人了！

根據您公司使用的CRM，從下列選擇。

    * [將Marketo與Salesforce.com整合](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [將Marketo與Microsoft Dynamics整合](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>您需要公司CRM管理員的協助，才能完成這些步驟。

## 新增追蹤代碼至您的網站{#add-tracking-code-to-your-website}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問將在您的IT設定說明文檔中提供Munchkin代碼說明。

Marketo有自訂追蹤JavaScript（稱為Munchkin），您可用來追蹤任何網頁上的人員活動。 Munchkin必須將您的網站整合至Marketo。 請依照下列步驟，將[Add Munchkin Tracking Code to Your Website](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)。

>[!NOTE]
>
>新增追蹤程式碼需要使用HTML的經驗。

您的所有設定步驟都結束。 只剩下投入使用Marketo!
