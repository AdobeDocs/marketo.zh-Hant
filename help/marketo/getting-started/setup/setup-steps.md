---
unique-page-id: 2949469
description: 設定步驟 — Marketo檔案 — 產品檔案
title: 設定步驟
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 0%

---

# 設定步驟 {#setup-steps}

**歡迎使用Marketo Engage！**

在開始使用Marketo之前，您需要完成一些步驟。

這些步驟包括：

* 一些基本帳戶設定
* 品牌化登陸頁面URL和電子郵件連結，以改善信任度和傳遞能力
* 正在同步您的CRM
* 將追蹤程式碼新增至您的公司網站

>[!NOTE]
>
>如果您的公司有以下需求，您才需要執行這些步驟 **Marketo的新手**. 如果沒有，則可能已完成設定。

部分步驟需要您的IT團隊協助。

>[!TIP]
>
>若您 [列印這份檢查清單](/help/marketo/getting-started/setup/setup-checklist.md){target="_blank"}，您可在完成專案時將其核取。

## 登入並建立其他Marketo使用者 {#log-in-and-create-additional-marketo-users}

登入Marketo [此處](https://app.marketo.com/){target="_blank"} 使用您透過電子郵件收到的認證。

![](assets/setup-steps-1.png)

恭喜！您現在在Marketo中，可以開始探索。 您可能會想要邀請行銷團隊中的同事加入您。 您可以新增使用者來完成此操作。

前往 **[!UICONTROL 管理員]** 區域。

>[!TIP]
>
>當您在這裡時，您可以按一下 **[!UICONTROL 我的帳戶]** 以變更您的帳戶和位置設定，以及設定新的訂閱名稱。

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**需要管理員許可權**

按一下 **[!UICONTROL 使用者和角色]**.

![](assets/setup-steps-3.png)

按一下 **[!UICONTROL 邀請新使用者]**.

![](assets/setup-steps-4.png)

填寫同事的電子郵件地址、名字和姓氏。 _可選擇設定存取到期日_. 按一下 **[!UICONTROL 下一個]**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>到期日非常適合短期的外部利害關係人或顧問，因為他們只需要短時間的Marketo存取權。

>[!NOTE]
>
>到期日到達時，使用者會收到到期通知，且帳戶會遭鎖定。

選取角色並按一下 **[!UICONTROL 下一個]**. 標準使用者可存取除「管理員」以外的所有區域。

![](assets/setup-steps-6.png)

>[!NOTE]
>
>除了五個內建角色外，您還可以建立自訂角色。 進一步瞭解 [管理使用者角色和許可權](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.

您可以隨意調整邀請文字。 按一下 **傳送**.

![](assets/setup-steps-7.png)

新使用者現在會列在 **[!UICONTROL 使用者]** 索引標籤上，和應該會收到一封電子郵件，其中包含建立密碼和登入的連結。 下一步！

![](assets/setup-steps-8.png)

## 設定您的授權支援連絡人 {#set-up-your-authorized-support-contacts}

您可能會收到Marketo支援的電子郵件，說明您是貴公司的Marketo客戶支援管理員。 若是如此，您可以設定 **授權支援聯絡人** 您的團隊的。 Marketo只有授權支援聯絡人可以直接透過 [Marketo支援入口網站](https://support.marketo.com){target="_blank"}.

>[!NOTE]
>
>您可以建立的支援聯絡人數量由您購買的套件決定。 此限制是在您來自Marketo支援的電子郵件中指定的。

授權支援聯絡檔案已移至Marketo社群。 請參閱 [本文](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}.

>[!NOTE]
>
>清單中只會顯示已登入Marketo社群的使用者。 如果您找不到該人員，請確定他們先登入社群。

## 使用CNAME自訂您的登陸頁面URL {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您的啟動電話會議期間，為您提供IT設定指示檔案。

>[!NOTE]
>
>**需要管理員許可權**

選擇登入頁面的CNAME。 部分範例：

    * **go**。[CompanyDomain].com
    * **www2**.[CompanyDomain].com
    * **lp**.[CompanyDomain].com

>[!TIP]
>
>保持簡短！ 較短的URL更容易記憶。 我們建議使用「前往」作為網域。

第一部分（粗體）為 `[LandingPageCNAME]`. 您在步驟5中需要它。

若要擷取您將會以登陸頁面CNAME取代的Munchkin ID，請前往管理區域。

![](assets/setup-steps-9.png)

按一下 **我的帳戶**.

![](assets/setup-steps-10.png)

複製 [!UICONTROL 帳戶字串] 從登入頁面設定。

![](assets/setup-steps-11.png)

這是 `[Munchkin ID]`. 儲存它。 您必須在步驟5中將其提供給IT。

設定您的網域設定，讓登陸頁面使用您公司的網域，而非Marketo （託管位置）。

## 確保電子郵件傳遞能力 {#ensure-email-deliverability}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您的啟動電話會議期間，為您提供IT設定指示檔案。

您可以採取幾項措施，確保電子郵件儘可能送達更多的人。

* **品牌化追蹤連結**. 您可以選擇CNAME，在您從Marketo加入的電子郵件連結中使用自己的網域(而不是Marketo)。 這加強了您的網域品牌化，並增加了與收件者的信任度和可遞送性。
* **將Marketo新增至您的公司電子郵件允許清單。** 在將電子郵件傳送給實際使用者之前，將測試電子郵件傳送給測試帳戶是常見的最佳做法。 透過將Marketo加入允許清單，您可以防止這些測試電子郵件被封鎖或標籤為垃圾訊息。
* **設定SPF和DKIM。** 這些技術可讓您的收件者確信，您的Marketo電子郵件不是垃圾郵件。 若要協助防止收件者的垃圾郵件篩選器拒絕您Marketo電子郵件，請按照以下步驟執行 [設定電子郵件傳遞能力的SPF和DKIM](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **為您的網域設定MX記錄。** MX記錄可讓您接收寄送電子郵件至之網域的郵件，以處理回覆及自動回應。 如果您從公司網域傳送，則可能已設定此專案。 如果沒有，您通常可以設定對應到您公司網域的MX記錄。
* **寄件者地址的建議設定。** 您必須在所有電子郵件行銷活動的「寄件者地址」中使用有效的、現有的和工作中的電子郵件網域。 設定公司網域的子網域比從公司網域傳送可能更有幫助。 這將確保企業郵件流中的問題不會影響您的Marketo郵件流，反之亦然。 此外，傳送郵件自 `something@nonexistentdomain.com` 將導致篩選或封鎖電子郵件。 寄件者寄件者地址中使用的任何網域都必須具備有效且正常運作的郵局主管@和濫用@帳戶。

如果您使用Google應用程式來託管公司電子郵件，則無法在您的網域下建立濫用@或郵遞員@電子郵件。 若要解決此問題，您需要建立名為「濫用」和「郵遞員」的群組。 屬於這些群組成員的使用者將會收到傳送至這些地址的電子郵件(例如postmaster@domain.com)。 建立群組的詳細指示可找到 [此處](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

選擇用於電子郵件追蹤連結的CNAME (選擇一個 _不同_ （從您在步驟3中選擇的登陸頁面CNAME）。 部分範例：

* go2。[CompanyDomain].com
* em.[CompanyDomain].com
* 哇！[CompanyDomain].com

第一部分是電子郵件追蹤CNAME， `[EmailTrackingCNAME]`. 您必須在步驟5中將其提供給IT。

>[!CAUTION]
>
>電子郵件和登陸頁面CNAME必須不同。 此外，請避免CNAME，例如「track」或「link」。 它通常被標籤為垃圾訊息

若要尋找Marketo追蹤連結，請前往 **[!UICONTROL 管理員]** 區域。

![](assets/setup-steps-12.png)

按一下 **[!UICONTROL 電子郵件]**.

![](assets/setup-steps-13.png)

複製 [!UICONTROL 追蹤連結] 來自您的電子郵件設定。

此 [!UICONTROL 追蹤連結] 格式為： `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

這是您的 `[MktoTrackingLink]`. 儲存它。 您必須在步驟5中將其提供給IT。

收集「來自」網域。 建立所有「寄件者」網域的清單(如 `[Sender]@[FromDomain].com`)，並計畫用於從Marketo傳送電子郵件。 多數情況下，只有一個選項。

例如，&#39;marketo.com，&#39; &#39;info.marketo.com，&#39;。 這些是 `[FromDomain1]`，`[FromDomain2]`等。 儲存它們。 您必須在步驟5中將其提供給IT。

您現在擁有傳送要求給IT所需的所有資訊！

## 要求IT人員設定通訊協定 {#ask-it-to-configure-protocols}

>[!NOTE]
>
>您是Launch Pack客戶嗎？ 您可以略過此步驟。 您的顧問會在您的啟動電話會議期間，為您提供IT設定指示檔案。

收集完所有必要資訊後，您就可以向IT傳送要求了。 您可以使用下列文字做為範本，將粗體文字取代為您自己的資訊。

[加入本文的連結](/help/marketo/getting-started/setup/configure-protocols-for-marketo.md).

將此文字貼到電子郵件中，並取代粗體預留位置：

>[!NOTE]
>
>請參閱上述步驟3和4，決定取代預留位置的文字。 請記住 `[LandingPageCNAME]` 和 `[EmailTrackingCNAME]` 必須不同。

`----------------------------------------------`

尊敬的IT管理員：

我們的行銷團隊現在正使用Marketo平台與我們的人員溝通。 為確保出色的電子郵件傳遞能力，我們需要進行下列變更：

`1)` 對於我們的登入頁面，新增DNS專案(CNAME) **[LandingPageCNAME]**.**[CompanyDomain]**.com，指向 **[Munchkin ID]**.mktoweb.com.

`2)` 針對電子郵件中的追蹤連結，新增DNS專案(CNAME) **[EmailTrackingCNAME]**.**[CompanyDomain]**.com，指向 **[MktoTrackingLink]**.

`3)` 將Marketo加入允許清單。

    *如果在電子郵件允許清單中使用IP位址，請新增下列的IP：
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
>如果您想要取得特定於您環境的IP允許清單的縮寫，請聯絡Marketo支援。

    *如果我們的反垃圾郵件系統使用「寄件者」網域，請新增以下內容：

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` 我們需要設定SPF和DKIM，以便Marketo有權代表我們傳送已簽署的電子郵件。

`a.` 若要設定SPF，請在我們的DNS專案中新增下列行：

在TXT中 **[來自網域]**： v=spf1 mx ip4：**[公司IP]**
<br/>包含： mktomail.com ~all

如果我們的DNS專案已經有現有的SPF記錄，只需新增下列內容即可：

include：mktomail.com

`[`Replace **來自網域** 使用您的電子郵件來自網域(例如： company.com)和 **CorpIP** 企業電子郵件伺服器的IP位址（例如：255.255.255.255）。  如果您要透過Marketo從多個網域傳送電子郵件，應讓IT人員為每個網域新增此行（一行）。`]`

`b.` 對於DKIM，請針對我們要設定的每個網域建立DNS資源記錄。 我們將簽署的每個網域的主機記錄和TXT值如下：

**`[DKIMDomain1]`**：主機記錄為 **`[HostRecord1]`** 且TXT值為 **[TXTValue1]**.

**`[DKIMDomain2]`**：主機記錄為 **`[HostRecord2]`** 且TXT值為 **`[TXTValue2]`**.

`[`複製 **主機記錄** 和 **TXTValue** 針對每個 **Dkimdomain** 您在遵循以下步驟後完成設定 [此處提供指示](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). 別忘了驗證中的每個網域 **管理員>電子郵件> DKIM** 在您的IT人員完成此步驟之後。`]`

`5)` 我們需要確保我們的FROM網域有有效的MX記錄 **[FromDomain1]**， **[FromDomain2]**&#x200B;等。 您能確認嗎？ 如果沒有，請設定以對應到我們的公司網域MX記錄。 這將確保我們能夠處理Marketo郵件的回覆/自動回應者。

完成這些步驟後請通知我，以便我使用Marketo完成設定程式。

感謝您！ 你是最棒的！

愛，

**`[Your Name]`**

`----------------------------------------------`

傳送電子郵件給IT。 我們瞭解IT可能需要一些時間才能完成這些工作。 您可以繼續步驟7，但請記住，您必須傳回步驟6才能完成Marketo設定。

## 完成Marketo設定後 {#complete-your-marketo-setup-after-it-finishes}

在IT完成其工作後，請依照下列步驟新增您的登陸頁面和電子郵件CNAME，並啟動DKIM簽署。

前往 **[!UICONTROL 管理員]** 新增登陸頁面CNAME的區域

![](assets/setup-steps-15.png)

選取登入頁面並按一下 **[!UICONTROL 編輯]** 在 [!UICONTROL 設定] 區域。

![](assets/setup-steps-16.png)

在欄位中輸入您的新網域名稱 **[!UICONTROL 登陸頁面的網域名稱]**. 其形式應為：

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

在 **[!UICONTROL 遞補內容]** 頁面欄位中，輸入當登陸頁面無法使用時，您希望人們前往的URL。 如果您沒有後援頁面，可以使用公司首頁。 在 **[!UICONTROL 首頁]** 欄位中，輸入您的公司網站。

![](assets/setup-steps-18.png)

在 [!UICONTROL 管理員] 區域，選取 **[!UICONTROL 電子郵件]** 新增電子郵件CNAME的方式

![](assets/setup-steps-19.png)

向下捲動至 [!UICONTROL 品牌化網域]. 選取您的網域並按一下 **[!UICONTROL 編輯]**.

![](assets/setup-steps-20.png)

在「網域」欄位中，輸入您的電子郵件追蹤網域。 其形式應為：

`[EmailTrackingCNAME].[CompanyDomain].com`. 按一下 **[!UICONTROL 儲存]**.

![](assets/setup-steps-21.png)

## 整合您的CRM {#integrate-your-crm}

這可能是您設定中最令人興奮的步驟 — 您應該使用所有您在CRM中儲存的銷售機會和聯絡人來填滿Marketo！

根據貴公司使用的CRM，從下列專案中選擇。

    * [整合Marketo與 [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [整合Marketo與 [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>您需要公司的CRM管理員協助才能完成這些步驟。

## 新增追蹤程式碼至您的網站 {#add-tracking-code-to-your-website}

>[!NOTE]
>
>您是否為 [!DNL Launch Pack] 客戶？ 您可以略過此步驟。 您的顧問會為您提供 [!DNL Munchkin] IT設定指示檔案中的程式碼指示。

Marketo有自訂追蹤JavaScript (稱為 [!DNL Munchkin])來追蹤個人在任何網頁上的活動。 [!DNL Munchkin] 需要將您的網站整合至Marketo。 請依照下列步驟執行 [新增 [!DNL Munchkin] 追蹤程式碼至您的網站](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>需要HTML體驗才能新增追蹤程式碼。

## 效能期望 {#performance-expectations}

Marketo的效能有何期望？ 視行銷活動的規模和複雜性而定，可能會有所不同。 但您可以預期效能等級與以下表格中的「標準」欄中所列的相同： [Marketo Engage產品說明](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. The "Performance" and "Performance Plus" columns refer to performance tier packages that provide [higher performance levels](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

您的所有設定步驟都已完成。 只剩下深入瞭解並使用Marketo了！
