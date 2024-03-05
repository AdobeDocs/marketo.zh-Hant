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
>[以SalesforceAppExchange安裝Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**需要管理員許可權。**

## 在Marketo Engage中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 若要在Marketo Engage中取得Marketo Sales Insight認證，請前往 **[!UICONTROL 管理員]** 區域並選取 **[!UICONTROL 銷售分析]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 按一下 **[!UICONTROL 編輯API設定]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 輸入您選擇的API秘密金鑰，然後按一下 **[!UICONTROL 儲存]**. 請勿使用&amp;符號(`&`)。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >您的API秘密金鑰就像您組織的密碼，應該是安全的。

1. 若要填入認證，請按一下 **[!UICONTROL 檢視]** 在 _[!UICONTROL Rest API設定]_ 面板。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 當您看到確認對話方塊時，請按一下 **[!UICONTROL 確定]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >保持此視窗開啟。 您稍後需要此資訊以進行Salesforce設定。

## 在Salesforce中設定Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，按一下 **[!UICONTROL 設定]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 搜尋「遠端站台」並選取 **[!UICONTROL 遠端站台設定]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 按一下 **[!UICONTROL 新增遠端站台]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. 輸入遠端站台名稱(可能類似於 `MarketoSoapAPI`)。 輸入遠端站台URL，這是您來自的Marketo主機URL。 _[!UICONTROL Soap API設定]_ 面板的Marketo Engage。 按一下 **[!UICONTROL 儲存]**. 您現在已建立Soap API的遠端站台設定。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. 按一下 **[!UICONTROL 新增遠端站台]** 再來一次。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. 輸入遠端站台名稱(可能類似於 `MarketoAPI`)。 輸入遠端站台URL，這是您的API URL，從 _[!UICONTROL Rest API設定]_ 面板的Marketo Engage。 按一下 **[!UICONTROL 儲存]**. 您現在已建立Rest API的遠端站台設定。

   >[!NOTE]
   >
   >_您_ 選擇您的 **[!UICONTROL 遠端站台名稱]** (`MarketoAPI` 此處使用)。 此 **[!UICONTROL 遠端站台URL]** 您可在「在Marketo中設定Sales Insight in Marketo」一節中步驟3之「編輯API設定」對話方塊的「主機」欄位中找到。

## 授予Sales Insight使用者對標準Salesforce物件的設定檔存取權 {#grant-sales-insight-users-profile-access}

由於Salesforce安全性增強，AppExchange套件無法再授與標準物件的許可權，而必須從Salesforce使用者的設定檔授與相關Salesforce物件的存取權。 若要授與必要的許可權，請依照下列步驟進行。

1. 按一下 **[!UICONTROL 設定]**.

1. 在快速尋找中搜尋「設定檔」。

1. 按一下 **[!UICONTROL 編輯]** ，位於您的Salesforce使用者正在使用的設定檔旁。

1. 在 _[!UICONTROL 標準物件許可權]_ 部分，啟用 **[!UICONTROL 讀取]** 存取下列物件： [!UICONTROL 銷售機會]， [!UICONTROL 連絡人]， [!UICONTROL 帳戶]、和 [!UICONTROL 商機].

1. 按一下&#x200B;**[!UICONTROL 保存]**。

## 自訂頁面配置 {#customize-page-layouts}

1. 按一下 **[!UICONTROL 設定]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 搜尋「頁面配置」並選取 **[!UICONTROL 頁面配置]** 在 **[!UICONTROL 銷售機會]**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 按一下 **[!UICONTROL Visualforce頁面]** 左側。 拖曳 **[!UICONTROL 章節]** 至配置圖底下 _[!UICONTROL 自訂連結]_ 區段。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 輸入「Marketo銷售分析」作為 **[!UICONTROL 區段名稱]**，選取 **[!UICONTROL 1欄]**，然後按一下 **[!UICONTROL 確定]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 拖放 **[!UICONTROL 銷售機會]** 放入新區段中。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此方塊的名稱會根據物件型別而變更。 例如，如果您正在修改「連絡人」的版面配置，則會顯示「連絡人」。

1. 按兩下 **[!UICONTROL 銷售機會]** 您剛才新增的區塊。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 編輯高度至 **450** 畫素並按一下 **[!UICONTROL 確定]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >檢查 **[!UICONTROL 顯示卷軸]** 如果您需要存取權才能捲動活動。

   >[!TIP]
   >
   >Accounts與Opportunities物件的建議高度為410畫素。

1. 按一下 **[!UICONTROL 欄位]** 左側。 然後搜尋並拖曳 **[!UICONTROL 急迫性]** 標籤放入 **[!UICONTROL Marketo Sales Insight]** 版面。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. 對這些欄位也重複上述步驟。

   * 上一個有趣的時刻
   * 上一個有趣的時刻日期
   * 上一個有趣時刻說明
   * 上一個有趣時刻來源
   * 上一個有趣的時刻型別
   * 依銷售顯示的最後一個活動
   * 上次參與次數（按銷售者）
   * MSI聯絡人ID
   * 相對分數
   * 相對分數值
   * 急迫性
   * 緊急值
   * 在Marketo中檢視

1. 按一下 **[!UICONTROL 儲存]** 完成後。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重複步驟5至7，新增Visualforce頁面區段和Sales Insight欄位 **[!UICONTROL 連絡人]**， **[!UICONTROL 帳戶]**、和 **[!UICONTROL 商機]**.

1. 重複步驟8至10，新增這些Sales Insight欄位 **[!UICONTROL 連絡人]**. 請務必儲存任何變更。

   * 上一個有趣的時刻
   * 上一個有趣的時刻日期
   * [!UICONTROL 上一個有趣時刻說明]
   * [!UICONTROL 上一個有趣時刻來源]
   * [!UICONTROL 上一個有趣的時刻型別]
   * [!UICONTROL 最後一個Marketo活動（依銷售分列）]
   * [!UICONTROL 銷售人員的最後一次Marketo參與]
   * [!UICONTROL MKTO銷售機會分數]
   * [!UICONTROL 相對分數]
   * [!UICONTROL 相對分數值]
   * [!UICONTROL 銷售分析]  — 開啟連絡人完整清單頁面
   * [!UICONTROL 急迫性]
   * [!UICONTROL 緊急值]

## 對應自訂人員欄位 {#map-custom-person-fields}

Marketo人員欄位必須對應至Salesforce聯絡人欄位，以確保轉換正常運作。 請依照下列步驟進行對應。

1. 按一下 **[!UICONTROL 設定]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 在搜尋列中搜尋「欄位」，然後按一下 **[!UICONTROL 欄位]** 在 **[!UICONTROL 銷售機會]**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 按一下 **[!UICONTROL 對應潛在客戶欄位]**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 按一下右側的下拉式清單 **[!UICONTROL 參與]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. 選取 **[!UICONTROL Contact.Engagement]** 在清單中。

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

1. 按一下 **[!UICONTROL 儲存]** 完成時。

## Marketo Sales Insight設定索引標籤 {#marketo-sales-insight-configuration-tab}

1. 在Salesforce中，按一下 **+** 標籤列末端，然後按一下 **[!UICONTROL Marketo銷售分析設定]**.

1. 從的Soap API面板複製認證 [Marketo的Sales Insight管理頁面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} 並將其貼到「Salesforce銷售分析設定」頁面的「Soap API」區段。

1. 從的Rest API面板複製認證 [Marketo的Sales Insight管理頁面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} 並貼到「Salesforce銷售分析設定」頁面的Rest API區段。

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

您應該能夠檢視銷售機會、聯絡人、帳戶和機會的Marketo銷售分析欄位。

>[!NOTE]
>
>如果診斷測試失敗， [新增更多欄位至您的頁面配置](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} 可能會修正問題。

>[!NOTE]
>
>對於帳戶，Sales Insight會包含所有電子郵件，但僅包含最近有趣的時刻、網頁活動和分數變更。

>[!MORELIKETHIS]
>
>* [優先順序、急迫性、相對分數和首選](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [將Marketo標籤新增至Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [將銷售分析存取權新增至設定檔](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
