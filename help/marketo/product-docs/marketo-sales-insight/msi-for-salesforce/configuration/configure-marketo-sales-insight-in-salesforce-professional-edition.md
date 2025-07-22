---
unique-page-id: 3571743
description: 瞭解如何在Marketo Professional Edition中設定Salesforce Sales Insight 。
title: 在Marketo Professional Edition中設定Salesforce Sales Insight
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 1%

---

# 在[!DNL Marketo Sales Insight] Professional Edition中設定[!DNL Salesforce] {#configure-marketo-sales-insight-in-salesforce-professional-edition}

完成下列步驟，在Salesforce Professional Edition中設定Marketo Sales Insight 。

>[!PREREQUISITES]
>
>* 在您的[!DNL Salesforce] Professional Edition中安裝Marketo。
>
>* 在[AppExchange [!DNL Marketo Sales Insight] 中 [!DNL Salesforce] 安裝](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}封裝

>[!NOTE]
>
>**需要系統管理員許可權。**

## 在Marketo Engage中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 若要從您的Marketo帳戶取得Marketo銷售Insight憑證，請開啟新的瀏覽器視窗。

1. 移至&#x200B;**[!UICONTROL Admin]**&#x200B;區域並選取&#x200B;**[!UICONTROL Sales Insight]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. 按一下「**[!UICONTROL Edit API Configuration]**」。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. 輸入您選擇的API秘密金鑰，然後按一下&#x200B;**[!UICONTROL Save]**。 請勿在您的API秘密金鑰中使用&amp;符號(`&`)。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >您的API秘密金鑰就像您組織的密碼，應該是安全的。

1. 若要填入認證，請按一下&#x200B;**[!UICONTROL View]**&#x200B;面板中的&#x200B;_[!UICONTROL Rest API Configuration]_。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. 當您看到確認對話方塊時，請按一下&#x200B;**[!UICONTROL OK]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## 在[!DNL Salesforce]中設定銷售Insight {#configure-sales-insight-in-salesforce}

1. 從Salesforce按一下&#x200B;**[!UICONTROL Setup]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. 搜尋「遠端站台」並選取&#x200B;**[!UICONTROL Remote Site Settings]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. 按一下「**[!UICONTROL New Remote Site]**」。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. 輸入遠端站台名稱（名稱可能類似於`MarketoSoapAPI`）。 輸入遠端網站URL，這是您在Marketo Engage的「Soap API設定」面板中的Marketo主機URL。 按一下&#x200B;**[!UICONTROL Save]**。 您現在已建立Soap API的遠端站台設定。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. 再按一下&#x200B;**[!UICONTROL New Remote Site]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. 輸入遠端網站名稱（類似「MarketoRestAPI」）。 輸入遠端網站URL，這是您在Marketo的Rest API設定面板中的API URL。 按一下&#x200B;**[!UICONTROL Save]**。 您現在已建立Rest API的遠端站台設定。

## 授予Sales Insight使用者設定檔存取標準Salesforce物件的許可權 {#grant-sales-insight-users-profile-access}

由於Salesforce安全性增強功能，AppExchange套件無法再授與標準物件的許可權，且必須從Salesforce使用者的設定檔授與相關Salesforce物件的存取權。 請依照下列步驟授與必要的許可權。

1. 按一下「**[!UICONTROL Setup]**」。

1. 在快速尋找中搜尋「設定檔」。

1. 按一下Salesforce使用者正在使用的設定檔旁的&#x200B;**[!UICONTROL Edit]**。

1. 在「標準物件許可權」區段下，啟用下列物件的「讀取」存取權：銷售機會、連絡人、帳戶和機會。

1. 按一下「**[!UICONTROL Save]**」。

## 自訂頁面配置 {#customize-page-layouts}

1. 按一下「**[!UICONTROL Setup]**」。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 搜尋「頁面配置」並選取&#x200B;**[!UICONTROL Page Layout]**&#x200B;下的&#x200B;**[!UICONTROL Leads]**。

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. 按一下左側的&#x200B;**[!UICONTROL Visualforce Pages]**。 將&#x200B;**[!UICONTROL Section]**&#x200B;拖曳至「自訂連結」區段下的配置。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 輸入「Marketo Sales Insight」做為&#x200B;**[!UICONTROL Section Name]**。 選取&#x200B;**[!UICONTROL 1-Column]**&#x200B;並按一下&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 將&#x200B;**[!UICONTROL Lead]**&#x200B;拖放至新區段。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此方塊的名稱會根據物件型別而變更。 例如，如果您正在修改「連絡人」的版面配置，則會顯示「連絡人」。

1. 連按兩下您剛才新增的&#x200B;**[!UICONTROL Lead]**&#x200B;區塊。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 將高度編輯為450畫素，然後按一下&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >若您需要捲動活動的存取權，請核取&#x200B;**[!UICONTROL Show scrollbars]**。

   >[!TIP]
   >
   >Accounts與Opportunities物件的建議高度為410畫素。

1. 按一下左側的&#x200B;**[!UICONTROL Fields]**。 然後搜尋&#x200B;**[!UICONTROL Engagement]**&#x200B;標籤並拖曳到&#x200B;**[!UICONTROL Marketo Sales Insight]**&#x200B;版面配置中。

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. 對下列欄位重複上述步驟：

   * [!UICONTROL Engagement]
   * [!UICONTROL Relative Score Value]
   * [!UICONTROL Urgency Value]
   * [!UICONTROL Last Interesting Moment Date]
   * [!UICONTROL Last Interesting Moment Desc]
   * [!UICONTROL Last Interesting Moment Source]
   * [!UICONTROL Last Interesting Moment Type]

1. 完成後，請按一下 **[!UICONTROL Save]**。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 若要新增&#x200B;**[!UICONTROL Contact]**、**[!UICONTROL Account]**&#x200B;和&#x200B;**[!UICONTROL Opportunity]**&#x200B;的Visualforce頁面區段，請重複步驟5至7。

1. 重複步驟8至10，為&#x200B;**[!UICONTROL Contact]**&#x200B;新增Sales Insight欄位。 進行變更後請務必儲存。

## 對應自訂人員欄位 {#map-custom-person-fields}

Marketo人員欄位必須對應至Salesforce聯絡人欄位，以確保轉換可正常運作。 請依照下列步驟進行對應。

1. 按一下「**[!UICONTROL Setup]**」。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 在搜尋列中搜尋「欄位」，然後按一下&#x200B;**[!UICONTROL Fields]**&#x200B;下方的&#x200B;**[!UICONTROL Leads]**。

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. 按一下「**[!UICONTROL Map Lead Fields]**」。

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. 按一下&#x200B;**[!UICONTROL Engagement]**&#x200B;右側的下拉式清單。

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. 在清單中選取&#x200B;**[!UICONTROL Contact.Engagement]**。

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. 同時重複並對應這些欄位。

   | Marketo人員自訂欄位 | Salesforce聯絡人自訂欄位 |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

   {style="table-layout:auto"}

1. 完成後，按一下「**[!UICONTROL Save]**」。

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketo Sales Insight設定索引標籤 {#marketo-sales-insight-configuration-tab}

1. 從Salesforce中，按一下標籤列結尾的&#x200B;**+**，然後按一下&#x200B;**[!UICONTROL Marketo Sales Insight Config]**。

1. 從[Marketo的Sales Insight管理頁面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}中的Soap API面板複製認證，並將其貼到Salesforce Sales Insight設定頁面的Soap API區段中。

1. 從&#x200B;**[!UICONTROL Rest API]** Marketo的Sales Insight管理頁面[中的](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}面板複製認證，並將其貼到Salesforce Sales Insight設定頁面的Rest API區段。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

您應該能夠檢視銷售機會、聯絡人、帳戶和機會的Marketo銷售Insight欄位。

>[!NOTE]
>
>如果診斷測試失敗，[新增更多欄位到您的頁面配置](https://nation.marketo.com/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"}可能會修正問題。

>[!NOTE]
>
>對於帳戶，Sales Insight會包含所有電子郵件，但僅包含最近有趣的時刻、網路活動和分數變更。

>[!MORELIKETHIS]
>
>* [優先順序、急迫性、相對分數和首選](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [新增Marketo索引標籤至 [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [將銷售Insight存取權新增至設定檔](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
