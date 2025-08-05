---
description: 設定步驟 - Marketo 文件 - 產品文件
short-description: 剛開始使用 Adobe Marketo Engage？了解深入使用前需要完成哪些步驟。
title: 設定步驟
feature: Getting Started
exl-id: 5f37da48-b2ed-4e48-a5a2-429149745085
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 2%

---

# 設定步驟 {#setup-steps}

**歡迎使用Adobe Marketo Engage！**

在您開始使用之前，請先完成一些步驟。

這些步驟包括：

* 品牌化您的登陸頁面URL和電子郵件連結，以改善信任度和傳遞能力
* 設定Marketo Engage的通訊協定
* 正在同步您的CRM
* 將追蹤程式碼新增至您的公司網站

>[!NOTE]
>
>如果您的公司是&#x200B;**Marketo的新手**，您才需要執行這些步驟。 如果沒有，則可能已完成設定。

部分步驟需要您的IT團隊協助。

## 確保電子郵件傳遞能力 {#ensure-email-deliverability}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您啟動電話時，為您提供IT設定指示檔案。

您可以採取幾項措施，確保電子郵件儘可能觸及更多的人。

* **將您的追蹤連結品牌化**。 您可以在來自Marketo的電子郵件中所包含的連結中，選擇使用您自己的網域(而非Marketo)的CNAME。 這加強了您的網域品牌，並增加了與收件者的信任度和可傳遞性。
* **將Marketo新增至您的公司電子郵件允許清單**。 通常的最佳實務是在傳送電子郵件給實際人員之前，先將測試電子郵件傳送給您的測試帳戶。 透過將Marketo加入允許清單，您可以防止這些測試電子郵件遭到封鎖或標籤為垃圾訊息。
* **設定SPF和DKIM**。 這些技術可確保您的收件者知道您的Marketo電子郵件不是垃圾郵件。 若要防止收件者的垃圾郵件篩選器拒絕您的Marketo電子郵件，請依照下列步驟[設定SPF和DKIM以傳遞電子郵件](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md)。
* **為您的網域設定MX記錄。** MX記錄可讓您接收您傳送電子郵件之網域的郵件，以處理回覆及自動回應。 如果您要從公司網域傳送，您可能已經設定好此專案。 如果沒有，您通常可以設定對應到您公司網域的MX記錄。
* **寄件者地址的建議設定。**&#x200B;您必須在所有電子郵件行銷活動的[寄件者地址]中使用有效的、現有的和工作中的電子郵件網域。 設定公司網域的子網域，而非從公司網域傳送可能有所助益。 這將確保企業郵件流中的問題不會影響您的Marketo郵件流，反之亦然。 此外，從`something@nonexistentdomain.com`傳送郵件將導致電子郵件被篩選或封鎖。 寄件者寄件者地址中使用的任何網域都必須具備有效且運作中的郵局主管@與濫用@帳戶。

如果您使用Google應用程式來託管公司電子郵件，則無法在您的網域下建立濫用@或郵遞員@電子郵件。 若要解決此問題，您需要建立名為「濫用」和「郵遞區長」的群組。 屬於這些群組成員的使用者將會收到傳送給這些地址的電子郵件（例如，<postmaster@domain.com>）。 您可以在[這裡](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}找到建立群組的詳細指示。

為電子郵件追蹤連結選擇一個CNAME （從您在步驟3中選擇的登陸頁面CNAME中選擇一個&#x200B;_不同的_）。 部分範例：

* go2。[CompanyDomain].com
* em.[CompanyDomain].com
* 哇！[CompanyDomain].com

第一部分是電子郵件追蹤CNAME `[EmailTrackingCNAME]`。 您需要將它授予IT。

>[!CAUTION]
>
>電子郵件和登陸頁面CNAME必須不同。 此外，請避免使用「追蹤」或「連結」之類的CNAME。 它經常被標籤為垃圾訊息

若要尋找您的Marketo追蹤連結，請前往&#x200B;**[!UICONTROL Admin]**&#x200B;區域。

![](assets/setup-steps-1.png)

按一下「**[!UICONTROL Email]**」。

![](assets/setup-steps-2.png)

從您的電子郵件設定複製[!UICONTROL Tracking Link]。

[!UICONTROL Tracking Link]的格式為： `mkto-[a-z][4 digits].com`。

![](assets/setup-steps-3.png)

這是您的`[MktoTrackingLink]`。 儲存它。 您必須在步驟5中將其提供給IT。

收集「來自」網域。 建立您打算用來從Marketo傳送電子郵件的所有「寄件者」網域清單（如`[Sender]@[FromDomain].com`）。 多數情況下只有一個。

例如，「marketo.com，」「info.marketo.com，」。 這些是`[FromDomain1]`、`[FromDomain2]`等。 儲存它們。 您必須在步驟5中將其提供給IT。

您現在擁有傳送要求給IT所需的所有資訊！

## 使用CNAME自訂您的登陸頁面URL {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您啟動電話時，為您提供IT設定指示檔案。

>[!NOTE]
>
>**需要管理員許可權**

為您的登入頁面選擇一個CNAME。 部分範例：

    * **執行**。[CompanyDomain].com
    * **www2**。[CompanyDomain].com
    * **lp**。[CompanyDomain].com

>[!TIP]
>
>保持簡短！ 較短的URL更容易記憶。 我們建議使用「前往」作為網域。

第一部分（粗體字）是`[LandingPageCNAME]`。 您在步驟5中需要它。

若要擷取您即將以登陸頁面CNAME取代的Munchkin ID，請移至&#x200B;**管理員**&#x200B;區域。

![](assets/setup-steps-4.png)

按一下&#x200B;**我的帳戶**。

![](assets/setup-steps-5.png)

從登入頁面設定複製[!UICONTROL Account String]。

![](assets/setup-steps-6.png)

這是`[Munchkin ID]`。 儲存它。 您必須在步驟5中將其提供給IT。

設定您的網域設定，讓登陸頁面使用您公司的網域，而非Marketo （託管位置）。

## 要求IT人員設定通訊協定 {#ask-it-to-configure-protocols}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您啟動電話時，為您提供IT設定指示檔案。

收集完所有必要資訊後，您就可以向IT傳送要求了。 您可以使用下列文字做為範本，將粗體文字取代為您自己的資訊。

[包含此文章的連結](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md)。

將此文字貼到電子郵件中，並取代粗體預留位置：

>[!NOTE]
>
>請參閱上述步驟3和4，決定取代預留位置的文字。 請記住，`[LandingPageCNAME]`和`[EmailTrackingCNAME]`必須不同。

`----------------------------------------------`

親愛的IT管理員：

我們的行銷團隊現在正使用Marketo平台與我們的人員溝通。 為確保出色的電子郵件傳遞能力，我們需要進行下列變更：

`1)`針對我們的登入頁面，新增&#x200B;**[LandingPageCNAME]**&#x200B;的DNS專案(CNAME)。**[CompanyDomain]**.com，指向&#x200B;**[Munchkin ID]**.mktoweb.com。

`2)`針對電子郵件中的追蹤連結，新增&#x200B;**[EmailTrackingCNAME]**&#x200B;的DNS專案(CNAME)。**[CompanyDomain]**.com，指向&#x200B;**[MktoTrackingLink]**。

`3)`允許清單Marketo。

    *如果我們在電子郵件允許清單中使用IP位址，請新增下列的IP：
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
>如果您想要取得特定環境的允許清單（IP的縮寫），請聯絡Marketo支援。

    *如果我們的反垃圾郵件系統使用[寄件者]網域，請新增這些網域：

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)`我們需要設定SPF和DKIM，因此Marketo有權代表我們傳送已簽署的電子郵件。

`a.`若要設定SPF，請在我們的DNS專案中新增下列行：

在TXT中&#x200B;**[來自網域]**： v=spf1 mx ip4：**[公司IP]**
<br/>包含： mktomail.com ~all

如果我們的DNS專案中已有現有的SPF記錄，只需新增下列內容即可：

include:mktomail.com

`[`將&#x200B;**來自網域**&#x200B;取代為您的來自網域的電子郵件(例如： company.com)，並將&#x200B;**CorpIP**&#x200B;取代為您的公司電子郵件伺服器的IP位址（例如： 255.255.255.255）。  如果您要透過Marketo從多個網域傳送電子郵件，請讓IT人員為每個網域新增此行（一行）。`]`

`b.`對於DKIM，請為每個我們要設定的網域建立DNS資源記錄。 我們將簽署的每個網域的主機記錄和TXT值如下：

**`[DKIMDomain1]`**：主機記錄為 **`[HostRecord1]`**，TXT 值為 **`[TXTValue1]`**。

**`[DKIMDomain2]`**：主機記錄為 **`[HostRecord2]`**，TXT 值為 **`[TXTValue2]`**。

`[`依照此處&#x200B;**的指示**&#x200B;複製您已設定的每個&#x200B;**DKIMDomain**&#x200B;的&#x200B;**HostRecord**&#x200B;和[TXTValue](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md)。 在您的IT人員完成此步驟後，別忘了驗證&#x200B;**管理員>電子郵件> DKIM**&#x200B;中的每個網域。`]`

`5)`我們需要確保我們的FROM網域&#x200B;**`[FromDomain1]`**、**`[FromDomain2]`**&#x200B;等有有效的MX記錄。 您能確認嗎？ 如果沒有，請設定對應至我們的企業網域MX記錄。 這將確保我們能夠處理Marketo郵件的回覆/自動回應者。

完成上述步驟後請通知我，以便我使用Marketo完成設定程式。

感謝支持！你是最棒的！

祝順心，

**`[Your Name]`**

`----------------------------------------------`

傳送電子郵件給IT。 我們瞭解，IT可能需要一些時間才能完成這些工作。 您可以繼續下一個步驟，但請記住，您必須返回此步驟才能完成Marketo Engage設定。

## 完成Marketo設定後 {#complete-your-marketo-setup-after-it-finishes}

IT完成工作後，請依照下列步驟新增登入頁面和電子郵件CNAME，並啟用DKIM簽署功能。

移至&#x200B;**[!UICONTROL Admin]**&#x200B;區域以新增您的登陸頁面CNAME

![](assets/setup-steps-7.png)

選取登入頁面，然後按一下&#x200B;**[!UICONTROL Edit]**&#x200B;區域中的[!UICONTROL Settings]。

![](assets/setup-steps-8.png)

在欄位&#x200B;**[!UICONTROL Domain Name for Landing Pages]**&#x200B;中輸入您的新網域名稱。 其形式應為：

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-9.png)

在&#x200B;**[!UICONTROL Fallback]**&#x200B;頁面欄位中，輸入當登陸頁面無法使用時，您希望人員前往的URL。 如果您沒有後援頁面，可以使用公司首頁。 在&#x200B;**[!UICONTROL Homepage]**&#x200B;欄位中，輸入您的公司網站。

![](assets/setup-steps-10.png)

在[!UICONTROL Admin]區域中，選取&#x200B;**[!UICONTROL Email]**&#x200B;以新增您的電子郵件CNAME

![](assets/setup-steps-11.png)

向下捲動至[!UICONTROL Branding Domains]。 選取您的網域並按一下&#x200B;**[!UICONTROL Edit]**。

![](assets/setup-steps-12.png)

在「網域」欄位中，輸入您的電子郵件追蹤網域。 其形式應為：

`[EmailTrackingCNAME].[CompanyDomain].com`。按一下「**[!UICONTROL Save]**」。

![](assets/setup-steps-13.png)

## 整合您的CRM {#integrate-your-crm}

這可能是您設定中最令人興奮的部分。 您應該在Marketo中填入所有您儲存在CRM中的潛在客戶和聯絡人！

請根據貴公司使用的CRM從下列專案中選擇。

* [將Marketo Engage與 [!DNL Salesforce.com]整合](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
* [將Marketo Engage與 [!DNL Microsoft Dynamics]整合](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

  >[!NOTE]
  >
  >您需要公司的CRM管理員協助才能完成這些步驟。

## 將追蹤程式碼新增至您的網站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>您是[!DNL Launch Pack]客戶嗎？ 您可以略過此步驟。 您的顧問會在您的IT設定指示檔案中提供[!DNL Munchkin]程式碼指示。

Marketo Engage有自訂追蹤JavaScript （稱為[!DNL Munchkin]），您可以使用它來追蹤任何網頁上的個人活動。 需要[!DNL Munchkin]才能將您的網站整合至Marketo。 請依照下列步驟[新增 [!DNL Munchkin] 追蹤程式碼至您的網站](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}。

>[!NOTE]
>
>若要新增追蹤程式碼，需有HTML的使用體驗。

## 效能期望 {#performance-expectations}

Marketo的效能表現如何？ 其可能會因行銷活動的規模和複雜性而異。 但您可在[Marketo Engage產品說明](https://helpx.adobe.com/tw/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}中找到的數個表格中，預期與「標準」欄中所概述的效能等級相等。 「效能」和「效能加上」欄是指提供[較高效能等級](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}的效能層級套件。

>[!MORELIKETHIS]
>
>* [設定Marketo Engage的通訊協定](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md)
>
>* [使用者設定](/help/marketo/getting-started/initial-setup/user-setup.md)
