---
unique-page-id: 2360368
description: 瞭解如何在Salesforce Enterprise/Unlimited版本中設定Marketo Sales Insight。
title: 在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 3cbefabe80778b0502eaecd733b5732fd9003316
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# 在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

完成下列步驟，在Salesforce Enterprise/Unlimited版本中設定Marketo Sales Insight。

>[!PREREQUISITES]
>
>[在SalesforceAppExchange中安裝Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**需要系統管理員許可權。**

## 在Marketo Engage中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 若要取得Marketo Engage中的Marketo Sales Insight認證，請移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域並選取&#x200B;**[!UICONTROL Sales Insight]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 按一下&#x200B;**[!UICONTROL 編輯API組態]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 輸入您選擇的API秘密金鑰，然後按一下&#x200B;**[!UICONTROL 儲存]**。 請勿在您的API秘密金鑰中使用&amp;符號(`&`)。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >您的API秘密金鑰就像您組織的密碼，應該是安全的。

1. 若要填入認證，請在&#x200B;_[!UICONTROL Rest API組態]_&#x200B;面板中按一下&#x200B;**[!UICONTROL 檢視]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 當您看到確認對話方塊時，請按一下[確定]。****

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >保持此視窗開啟。 您稍後需要此資訊以進行Salesforce設定。

## 在Salesforce中設定Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，按一下&#x200B;**[!UICONTROL 設定]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 搜尋「遠端站台」並選取&#x200B;**[!UICONTROL 遠端站台設定]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 按一下&#x200B;**[!UICONTROL 新增遠端站台]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. 輸入遠端站台名稱（名稱可能類似於`MarketoSoapAPI`）。 輸入遠端站台URL，這是Marketo Engage中&#x200B;_[!UICONTROL Soap API設定]_&#x200B;面板的Marketo主機URL。 按一下&#x200B;**[!UICONTROL 儲存]**。 您現在已建立Soap API的遠端站台設定。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. 再按一下&#x200B;**[!UICONTROL 新增遠端站台]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. 輸入遠端站台名稱（名稱可能類似於`MarketoAPI`）。 輸入遠端站台URL，這是您從&#x200B;_[!UICONTROL Rest API組態]_&#x200B;面板的API URL (Marketo Engage)。 按一下&#x200B;**[!UICONTROL 儲存]**。 您現在已建立Rest API的遠端站台設定。

   >[!NOTE]
   >
   >_您_&#x200B;選擇您的&#x200B;**[!UICONTROL 遠端站台名稱]** （`MarketoAPI`在此使用）。 在「在Marketo中設定Sales Insight」一節的步驟3「編輯API設定」對話方塊的「Marketo主機」欄位中，可以找到&#x200B;**[!UICONTROL 遠端網站URL]**。

## 授予Sales Insight使用者對標準Salesforce物件的設定檔存取權 {#grant-sales-insight-users-profile-access}

由於Salesforce安全性增強，AppExchange套件無法再授與標準物件的許可權，而必須從Salesforce使用者的設定檔授與相關Salesforce物件的存取權。 若要授與必要的許可權，請依照下列步驟進行。

1. 按一下&#x200B;**[!UICONTROL 設定]**。

1. 在快速尋找中搜尋「設定檔」。

1. 按一下Salesforce使用者正在使用的設定檔旁的&#x200B;**[!UICONTROL 編輯]**。

1. 在&#x200B;_[!UICONTROL 標準物件許可權]_&#x200B;區段下，啟用下列物件的&#x200B;**[!UICONTROL 讀取]**&#x200B;存取權： [!UICONTROL 潛在客戶]、[!UICONTROL 連絡人]、[!UICONTROL 帳戶]以及[!UICONTROL 機會]。

1. 按一下&#x200B;**[!UICONTROL 保存]**。

## 自訂頁面配置 {#customize-page-layouts}

1. 按一下&#x200B;**[!UICONTROL 設定]**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 搜尋「版面配置」並選取&#x200B;**[!UICONTROL 銷售機會]**&#x200B;下的&#x200B;**[!UICONTROL 版面配置]**。

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 按一下左側的&#x200B;**[!UICONTROL Visualforce頁面]**。 將&#x200B;**[!UICONTROL 區段]**&#x200B;拖曳至&#x200B;_[!UICONTROL 自訂連結]_&#x200B;區段下的配置。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 輸入「Marketo Sales Insight」作為&#x200B;**[!UICONTROL 區段名稱]**，選取&#x200B;**[!UICONTROL 1 — 欄]**，然後按一下&#x200B;**[!UICONTROL 確定]**。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 將&#x200B;**[!UICONTROL 銷售機會]**&#x200B;拖放至新的區段。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此方塊的名稱會根據物件型別而變更。 例如，如果您正在修改「連絡人」的版面配置，則會顯示「連絡人」。

1. 連按兩下您剛新增的&#x200B;**[!UICONTROL 銷售機會]**&#x200B;區塊。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 將高度編輯為&#x200B;**450**&#x200B;畫素，然後按一下&#x200B;**[!UICONTROL 確定]**。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >如果您需要捲動活動的存取許可權，請核取&#x200B;**[!UICONTROL 顯示卷軸]**。

   >[!TIP]
   >
   >Accounts與Opportunities物件的建議高度為410畫素。

1. 按一下左側的&#x200B;**[!UICONTROL 欄位]**。 然後搜尋&#x200B;**[!UICONTROL 急迫性]**&#x200B;標籤，並將其拖曳至&#x200B;**[!UICONTROL Marketo銷售分析]**&#x200B;版面配置。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. 對這些欄位也重複上述步驟。

   * 上一個有趣的時刻
   * 上一個有趣的時刻日期
   * 上一個有趣時刻說明
   * Source最後有趣的時刻
   * 上一個有趣的時刻型別
   * 依銷售顯示的最後一個活動
   * 上次參與次數（按銷售者）
   * MSI聯絡人ID
   * 相對分數
   * 相對分數值
   * 急迫性
   * 緊急值
   * 在Marketo中檢視

1. 完成時，按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重複步驟5至7，新增&#x200B;**[!UICONTROL 連絡人]**、**[!UICONTROL 帳戶]**&#x200B;和&#x200B;**[!UICONTROL 商機]**&#x200B;的Visualforce頁面區段和Sales Insight欄位。

1. 重複步驟8至10，為&#x200B;**[!UICONTROL 連絡人]**&#x200B;新增這些銷售分析欄位。 請務必儲存任何變更。

   * 上一個有趣的時刻
   * 上一個有趣的時刻日期
   * [!UICONTROL 上一個有趣的時刻Desc]
   * [!UICONTROL Source上一個有趣的時刻]
   * [!UICONTROL 上一個有趣的時刻型別]
   * [!UICONTROL 銷售人員最後的Marketo活動]
   * [!UICONTROL 銷售人員的最後一次Marketo參與]
   * [!UICONTROL MKTO銷售機會分數]
   * [!UICONTROL 相對分數]
   * [!UICONTROL 相對分數值]
   * [!UICONTROL 銷售分析] — 開啟連絡人完整清單頁面
   * [!UICONTROL 急迫性]
   * [!UICONTROL 緊急值]

## 對應自訂人員欄位 {#map-custom-person-fields}

Marketo人員欄位必須對應至Salesforce聯絡人欄位，以確保轉換正常運作。 請依照下列步驟進行對應。

1. 按一下&#x200B;**[!UICONTROL 設定]**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 在搜尋列中搜尋「欄位」，然後按一下&#x200B;**[!UICONTROL 銷售機會]**&#x200B;下的&#x200B;**[!UICONTROL 欄位]**。

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 按一下&#x200B;**[!UICONTROL 對應潛在客戶欄位]**。

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 按一下&#x200B;**[!UICONTROL 參與]**&#x200B;右側的下拉式清單。

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. 在清單中選取&#x200B;**[!UICONTROL Contact.Engagement]**。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. 重複並對應這些欄位。

   | Marketo人員自訂欄位 | Salesforce聯絡人自訂欄位 |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

1. 完成時，按一下&#x200B;**[!UICONTROL 儲存]**。

## Marketo Sales Insight設定索引標籤 {#marketo-sales-insight-configuration-tab}

1. 在Salesforce中，按一下標籤列結尾的&#x200B;**+**，然後按一下&#x200B;**[!UICONTROL Marketo Sales Insight Config]**。

1. 從[Marketo的Sales Insight Admin頁面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}中的Soap API面板複製認證，並將其貼到Salesforce Sales Insight設定頁面的Soap API區段中。

1. 從[Marketo的Sales Insight Admin頁面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}中的Rest API面板複製認證，並將其貼到Salesforce Sales Insight設定頁面的Rest API區段中。

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

您應該能夠檢視銷售機會、聯絡人、帳戶和機會的Marketo銷售分析欄位。

>[!NOTE]
>
>如果診斷測試失敗，[新增更多欄位到您的頁面配置](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"}可能會修正問題。

>[!NOTE]
>
>對於帳戶，Sales Insight會包含所有電子郵件，但僅包含最近有趣的時刻、網頁活動和分數變更。

>[!MORELIKETHIS]
>
>* [優先順序、急迫性、相對分數和首選](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [將Marketo索引標籤新增至Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [將銷售分析存取權新增至設定檔](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
