---
description: 設定步驟 - Marketo 文件 - 產品文件
short-description: 剛開始使用 Adobe Marketo Engage？了解深入使用前需要完成哪些步驟。
title: 設定步驟
feature: Getting Started
exl-id: 5f37da48-b2ed-4e48-a5a2-429149745085
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 100%

---

# 設定步驟 {#setup-steps}

**歡迎使用 Adobe Marketo Engage！**

在您開始探索前，您需要完成幾個步驟。

這些步驟包括：

* 將您的登陸頁面 URL 和電子郵件連結品牌化，以提升信任度和傳遞能力
* 設定 Marketo Engage 的通訊協定
* 同步處理您的 CRM
* 將追蹤代碼新增至您的公司網站

>[!NOTE]
>
>如果您的公司是&#x200B;**Marketo 的新使用者**，您才需要進行這些步驟。如果不是，則可能已完成設定。

部分步驟需要您的 IT 團隊協助。

## 確保電子郵件傳遞能力 {#ensure-email-deliverability}

>[!NOTE]
>
>您是否為 Launch Pack 客戶？您可以略過此步驟。您的顧問會在您啟動電話時，為您提供 IT 設定指示的文件。

您可以採取幾項措施來確保電子郵件盡可能觸及更多人。

* **讓您的追蹤連結具品牌識別**。您可以選擇 CNAME，以便在在 Marketo 電子郵件中所包含的連結中使用您自己的網域 (而不是 Marketo 的網域)。這可加強您的網域品牌化，並增加與收件者的信任度及傳遞能力。
* **將 Marketo 新增至您的公司電子郵件允許清單**。常見的最佳做法是在傳送電子郵件給實際人員之前，先將測試電子郵件傳送給您的測試帳戶。透過將 Marketo 加入允許清單，您可以防止這些測試電子郵件遭到封鎖或被加上垃圾郵件的旗標。
* **設定 SPF 和 DKIM**。這些技術可確保您的收件者知道您的 Marketo 電子郵件並非垃圾郵件。若要防止收件者的垃圾郵件篩選器拒絕您的 Marketo 電子郵件，請依照下列步驟[設定 SPF 和 DKIM 以提升電子郵件傳遞能力](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md)。
* **設定網域的 MX 記錄。** MX 記錄可讓您在寄送電子郵件的網域上接收郵件，以便處理回覆與自動回覆。如果您正從公司網域傳送，則有可能已經完成此設定。如果沒有，您通常可將其設定為對應至您的公司網域 MX 記錄。
* **寄件者地址的建議設定。**&#x200B;您必須在所有電子郵件行銷活動的寄件者地址中使用有效、現存且可正常運作的電子郵件網域。與其使用公司網域傳送電子郵件，設定公司網域的子網域可能更有效益。這可確保公司郵件流中的問題不會對您的 Marketo 郵件流造成影響，反之亦然。此外，從 `something@nonexistentdomain.com` 傳送郵件會導致電子郵件遭到篩選或封鎖。寄件者的寄件者地址中所使用的任何網域都必須具有有效且可正常運作的 postmaster@ 和 abuse@ 帳戶。

如果您使用 Google Apps 來託管公司電子郵件，則無法在您的網域下建立 abuse@ 或 postmaster@ 電子郵件。若要解決此問題，您需要建立名為「abuse」和「postmaster」的群組。屬於這些群組成員的使用者會收到傳送至這些地址的電子郵件 (例如，<postmaster@domain.com>)。如需建立群組的詳細指示，可參閱[這裡](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}。

為電子郵件追蹤連結選擇 CNAME (選擇一個與您在步驟 3 中選擇的登陸頁面 CNAME _不同的_ CNAME)。部分範例：

* go2。[CompanyDomain].com
* em。[CompanyDomain].com
* wow。[CompanyDomain].com

第一部分是電子郵件追蹤 CNAME，`[EmailTrackingCNAME]`。您需要將這個資料給 IT。

>[!CAUTION]
>
>電子郵件和登陸頁面 CNAME 必須不一樣。此外，請避免使用「track」或「link」之類的 CNAME。這通常會被標示為垃圾郵件

若要尋找您的 Marketo 追蹤連結，請前往 **[!UICONTROL Admin]** 區域。

![](assets/setup-steps-1.png)

按一下「**[!UICONTROL Email]**」。

![](assets/setup-steps-2.png)

從您的電子郵件設定複製 [!UICONTROL Tracking Link]。

[!UICONTROL Tracking Link] 的格式為：`mkto-[a-z][4 digits].com`。

![](assets/setup-steps-3.png)

這是您的 `[MktoTrackingLink]`。請將其儲存。您在步驟 5 中需要將這個資料提供給 IT。

收集「寄件者」網域。建立包含所有您計畫用於從 Marketo 寄送電子郵件的「寄件者」網域 (如 `[Sender]@[FromDomain].com`) 的清單。多數情況下只有一個。

例如，「marketo.com,」「info.marketo.com,」。這些是 `[FromDomain1]`、`[FromDomain2]` 等。請將其儲存。您在步驟 5 中需要將這些資料提供給 IT。

您現在有了傳送要求給 IT 所需的所有資訊！

## 使用 CNAME 自訂您的登陸頁面 URL {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>您是否為 Launch Pack 客戶？您可以略過此步驟。您的顧問會在您啟動電話時，為您提供 IT 設定指示的文件。

>[!NOTE]
>
>**需要管理員權限**

為您的登陸頁面選擇 CNAME。部分範例：

    * **go**。[CompanyDomain].com
    * **www2**。[CompanyDomain].com
    * **lp**。[CompanyDomain].com

>[!TIP]
>
>請保持簡短！較短的 URL 更容易記憶。我們建議使用「go」作為網域。

第一部分 (粗體字) 是 `[LandingPageCNAME]`。您在步驟 5 中會需要這個資料。

若要擷取您即將以登陸頁面 CNAME 取代的 Munchkin ID，請移至&#x200B;**管理員**&#x200B;區域。

![](assets/setup-steps-4.png)

按一下&#x200B;**我的帳戶**。

![](assets/setup-steps-5.png)

從登陸頁面設定複製 [!UICONTROL Account String]。

![](assets/setup-steps-6.png)

這是 `[Munchkin ID]`。請將其儲存。您在步驟 5 中需要將這個資料提供給 IT。

設定您的網域設定，讓登陸頁面使用您公司的網域，而非 Marketo 的網域 (託管位置)。

## 要求 IT 人員設定通訊協定 {#ask-it-to-configure-protocols}

>[!NOTE]
>
>您是否為 Launch Pack 客戶？您可以略過此步驟。您的顧問會在您啟動電話時，為您提供 IT 設定指示的文件。

收集完所有必要資訊後，您就準備好可向 IT 傳送要求了。您可以使用下列文字作為範本，以您自己的資訊取代粗體文字。

[包含本文的連結](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md)。

將這段文字貼到電子郵件中，並取代粗體的預留位置：

>[!NOTE]
>
>請查看上述步驟 3 和 4，來決定要取代預留位置的文字。請謹記，`[LandingPageCNAME]` 和 `[EmailTrackingCNAME]` 必須不一樣。

`----------------------------------------------`

IT 管理員您好：

我們的行銷團隊現在正使用 Marketo 平台與我們的人員溝通。為確保絕佳的電子郵件傳遞能力，我們需要進行下列變更：

`1)`對於我們的登陸頁面，請為 **[LandingPageCNAME]** 新增 DNS 項目 (CNAME)。**[CompanyDomain]**.com，會指向 **[Munchkin ID]**.mktoweb.com。

`2)`對於電子郵件中的追蹤連結，請為 **[EmailTrackingCNAME]** 新增 DNS 項目 (CNAME)。**[CompanyDomain]**.com，會指向 **[MktoTrackingLink]**。

`3)`允許清單 Marketo。

    *如果我們在電子郵件允許清單中使用 IP 位址，請將下列 IP 新增至清單：
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    94.236.119.0/26

>[!NOTE]
>
>如需您的環境的特定 IP 縮寫清單，請和 Marketo 支援聯繫。

    * 如果我們的反垃圾郵件系統使用寄件者網域，請新增這些：

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)`我們需要設定 SPF 和 DKIM，因此 Marketo 有權代表我們傳送已簽署的電子郵件。

`a.` 若要設定 SPF，請將下面一行新增至我們的 DNS 項目：

IN  TXT **[From Domain]**:  v=spf1 mx ip4:**[Corporate IP(s)]**
<br/>include: mktomail.com ~all

如果在我們的 DNS 項目中已經有現有的 SPF 記錄，則只要新增以下內容即可：

include:mktomail.com

`[`將 **寄件者網域**&#x200B;以您的電子郵件寄件者網域 (例如：company.com) 取代，並將 **CorpIP** 以您的公司電子郵件伺服器的 IP 位址取代 (例如：255.255.255.255)。如果您要透過 Marketo 從多個網域傳送電子郵件，請要求 IT 人員為每個網域新增此行 (在同一行)。`]`

`b.`對於 DKIM，請為每個我們要設定的網域建立 DNS 資源記錄。下列為我們將簽署的每個網域的主機記錄和 TXT 值：

**`[DKIMDomain1]`**：主機記錄為 **`[HostRecord1]`**，TXT 值為 **`[TXTValue1]`**。

**`[DKIMDomain2]`**：主機記錄為 **`[HostRecord2]`**，TXT 值為 **`[TXTValue2]`**。

`[`請依照[此處的指示](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)為您已設定的每個 **DKIMDomain** 複製 **HostRecord** 和 **TXTValue**。IT 人員完成此步驟後，別忘了在&#x200B;**「管理員 > 電子郵件 > DKIM」**&#x200B;中驗證每個網域。`]`

`5)`我們需要確保我們的寄件者網域 **`[FromDomain1]`**、**`[FromDomain2]`** 等都有有效的 MX 記錄。是否可以確認？如果不可以，請設定以對應至我們的公司網域 MX 記錄。這會確保我們可以處理 Marketo 郵件的回覆/自動回覆者。

完成上述步驟後請通知我，以便我可以使用 Marketo 完成設定流程。

謝謝您！你們是最棒的！

謹致

**`[Your Name]`**

`----------------------------------------------`

請傳送該電子郵件給 IT。我們了解，IT 可能需要一些時間才能完成這些工作。您可以繼續進行下一個步驟，但請謹記，您必須返回此步驟才能完成 Marketo Engage 設定。

## IT 完成後請完成您的 Marketo 設定 {#complete-your-marketo-setup-after-it-finishes}

IT 完成工作後，請依照下列步驟新增您的登陸頁面和電子郵件 CNAME，並啟用 DKIM 簽署功能。

移至 **[!UICONTROL Admin]** 區域，新增您的登陸頁面 CNAME

![](assets/setup-steps-7.png)

選取登陸頁面，然後按一下 [!UICONTROL Settings] 區域中的 **[!UICONTROL Edit]**。

![](assets/setup-steps-8.png)

在欄位 **[!UICONTROL Domain Name for Landing Pages]** 中輸入您的新網域名稱。其形式應為：

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-9.png)

在 **[!UICONTROL Fallback]** 頁面欄位中，輸入當登陸頁面無法使用時您希望人員前往的 URL。如果您沒有後援頁面，可以使用公司首頁。在 **[!UICONTROL Homepage]** 欄位中，輸入您的公司網站。

![](assets/setup-steps-10.png)

在 [!UICONTROL Admin] 區域中，選取 **[!UICONTROL Email]** 以新增您的電子郵件 CNAME

![](assets/setup-steps-11.png)

向下捲動至 [!UICONTROL Branding Domains]。選取您的網域，然後按一下 **[!UICONTROL Edit]**。

![](assets/setup-steps-12.png)

在「網域」欄位中，輸入您的電子郵件追蹤網域。其形式應為：

`[EmailTrackingCNAME].[CompanyDomain].com`。按一下「**[!UICONTROL Save]**」。

![](assets/setup-steps-13.png)

## 整合您的 CRM {#integrate-your-crm}

這可能是您的設定中最令人興奮的部分。您現在應該在 Marketo 中填入所有您在 CRM 中已儲存的銷售線索和聯絡人！

請依據貴公司使用的 CRM 從以下選項中進行選擇。

* [將 Marketo Engage 與  [!DNL Salesforce.com] 整合](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
* [將 Marketo Engage 與  [!DNL Microsoft Dynamics] 整合](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

  >[!NOTE]
  >
  >您需要公司的 CRM 管理員協助才能完成這些步驟。

## 將追蹤代碼新增至您的網站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>您是否為 [!DNL Launch Pack] 客戶？您可以略過此步驟。您的顧問會在您的 IT 設定指示文件中提供 [!DNL Munchkin] 代碼指示。

Marketo Engage 具有自訂的追蹤 JavaScript (稱為 [!DNL Munchkin])，您可以將其用於追蹤任何網頁上的人員活動。需要 [!DNL Munchkin] 才能將您的網站整合至 Marketo。請依照下列步驟進行，以[新增 [!DNL Munchkin] 追蹤代碼至您的網站](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}。

>[!NOTE]
>
>若要新增追蹤代碼，需要具備 HTML 使用經驗。

## 效能期望 {#performance-expectations}

您對於 Marketo 的效能有何期望？這可能會因行銷活動的規模和複雜性而異。但您可預期其效能等級會和在 [Marketo Engage 產品說明](https://helpx.adobe.com/tw/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}中所找到的幾個表格的「標準」欄中所概述的相當。「Performance」和「Performance Plus」欄指提供[較高效能等級](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}的效能層級套件。

>[!MORELIKETHIS]
>
>* [設定 Marketo Engage 的通訊協定](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md)
>
>* [使用者設定](/help/marketo/getting-started/initial-setup/user-setup.md)
