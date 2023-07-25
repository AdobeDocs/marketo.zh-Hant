---
unique-page-id: 2360368
description: 在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight - Marketo檔案 — 產品檔案
title: 在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# 在Salesforce Enterprise/Unlimited中設定Marketo Sales Insight {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

以下是設定Salesforce Enterprise/Unlimited Editions中Marketo Sales Insight的必要步驟。 讓我們開始吧。

>[!PREREQUISITES]
>
>[在SalesforceAppExchange中安裝Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**需要管理員許可權**

## 在Marketo中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 在Marketo中取得您的MSI認證。 前往管理區域並選取 **銷售分析**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 按一下 **編輯API設定**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 輸入您選擇的API秘密金鑰，然後按一下 **儲存**. 請勿在您的API秘密金鑰中使用&amp;符號。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >您的API秘密金鑰就像您組織的密碼，應該是安全的。

1. 按一下 **檢視** 在「Rest API設定」面板中填入認證。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 您將會看到確認快顯視窗。 按一下 **確定**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >保持此視窗開啟。 您稍後將需要此資訊到Salesforce。

## 在Salesforce中設定Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，按一下 **設定**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 搜尋「遠端站台」並選取 **遠端站台設定**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 按一下 **新增遠端站台**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. 輸入遠端網站名稱（可能類似「MarketoSoapAPI」）。 輸入遠端網站URL，這是您在Marketo的「Soap API設定」面板中的Marketo主機URL。 按一下 **儲存**. 您現在已建立Soap API的遠端站台設定。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. 按一下 **新增遠端站台** 再來一次。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. 輸入遠端網站名稱（類似「MarketoAPI」）。 輸入遠端網站URL，這是您從Marketo的Rest API設定面板取得的API URL。 按一下 **儲存**. 您現在已建立Rest API的遠端站台設定。

   >[!NOTE]
   >
   >_您_ 選擇您的 **遠端站台名稱** （此處使用MarketoAPI）。 此 **遠端網站URL** 您可在「在Marketo中設定Sales Insight 」一節中步驟3的「編輯API設定」對話方塊的「Marketo主機」欄位中找到。

## 自訂頁面配置 {#customize-page-layouts}

1. 按一下 **設定**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 搜尋「頁面配置」並選取 **頁面配置** 在 **銷售機會**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 按一下 **Visualforce頁面** 左側。 拖曳 **章節** 至自訂連結區段底下的配置。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 輸入「Marketo銷售分析」作為 **區段名稱**. 選取 **1欄** 並按一下 **確定**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 拖放 **銷售機會** 放入新區段中。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此方塊的名稱會根據物件型別而變更。 例如，如果您正在修改「連絡人」的頁面配置，則會顯示「連絡人」。

1. 連按兩下 **銷售機會** 您剛才新增的區塊。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 編輯高度至 **450** 畫素並按一下 **確定**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Check **顯示卷軸** 如果您需要存取權才能捲動活動。

   >[!TIP]
   >
   >我們建議將Accounts和Opportunities物件的高度設為410畫素。

1. 按一下 **欄位** 左側。 然後搜尋並拖曳 **急迫性** 標籤到 **Marketo Sales Insight** 版面。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. 對這些欄位也重複上述步驟。

   <table> 
    <tbody> 
     <tr> 
      <td>上一個有趣時刻</td> 
     </tr> 
     <tr> 
      <td>上一個有趣時刻日期</td> 
     </tr> 
     <tr> 
      <td>上一個有趣時刻說明</td> 
     </tr> 
     <tr> 
      <td>上一個有趣時刻來源</td> 
     </tr> 
     <tr> 
      <td>上一個有趣時刻型別</td> 
     </tr> 
     <tr> 
      <td>上次Marketo活動（依銷售）</td> 
     </tr> 
     <tr> 
      <td>銷售人員的最後Marketo參與</td> 
     </tr> 
     <tr> 
      <td>MSI連絡人ID</td> 
     </tr> 
     <tr> 
      <td>相對分數</td> 
     </tr> 
     <tr> 
      <td>相對分數值</td> 
     </tr> 
     <tr> 
      <td>急迫性</td> 
     </tr> 
     <tr> 
      <td>緊急值</td> 
     </tr> 
     <tr> 
      <td>在Marketo中檢視</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **儲存** 完成後。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重複步驟5至7，新增Visualforce頁面區段和Sales Insight欄位 **連絡人**， **帳戶** 和 **機會**.

1. 重複步驟8至10，從下列清單中新增Sales Insight欄位 **連絡人**. 請務必儲存任何變更。

<table> 
    <tbody> 
     <tr> 
      <td>上一個有趣時刻</td> 
     </tr> 
     <tr> 
      <td>上一個有趣時刻日期</td> 
     </tr> 
     <tr> 
      <td>上一個有趣時刻說明</td> 
     </tr> 
     <tr> 
      <td>上一個有趣時刻來源</td> 
     </tr> 
     <tr> 
      <td>上一個有趣時刻型別</td> 
     </tr> 
     <tr> 
      <td>上次Marketo活動（依銷售）</td> 
     </tr> 
     <tr> 
      <td>銷售人員的最後Marketo參與</td> 
     </tr> 
     <tr> 
      <td>MKTO銷售機會分數</td> 
     </tr> 
     <tr> 
      <td>相對分數</td> 
     </tr> 
     <tr> 
      <td>相對分數值</td> 
     </tr> 
     <tr> 
      <td>銷售分析 — 開啟連絡人完整清單頁面</td> 
     </tr> 
     <tr> 
      <td>急迫性</td> 
     </tr> 
     <tr> 
      <td>緊急值</td> 
     </tr> 
    </tbody> 
   </table>

## 對應自訂人員欄位 {#map-custom-person-fields}

Marketo人員欄位需要對應至Salesforce聯絡人欄位，以確保轉換正常運作。 方法如下。

1. 按一下 **設定**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 在搜尋列中搜尋「欄位」，然後按一下 **欄位** 在 **銷售機會**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 按一下 **對應潛在客戶欄位**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 按一下右側的下拉式清單 **參與**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. 選取 **Contact.Engagement** 在清單中。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. 重複並對應這些欄位。

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Marketo人員自訂欄位</th> 
      <th colspan="1" rowspan="1">Salesforce聯絡人自訂欄位</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>參與</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>相對分數值</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Relative Score值</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>緊急值</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Urgency值</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>上一個有趣時刻日期</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment日期</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>上一個有趣時刻說明</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Desc</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>上一個有趣時刻來源</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Source</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>上一個有趣時刻型別</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Type</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **儲存** 完成時。

## Marketo Sales Insight設定標籤 {#marketo-sales-insight-configuration-tab}

1. 在Salesforce中，按一下 **+** 標籤列末端，然後按一下 **Marketo銷售分析設定**.

1. 從中的Soap API面板複製認證 [Marketo的Sales Insight管理頁面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} 並將它們貼到「Salesforce銷售分析設定」頁面的Soap API區段中。

1. 從的Rest API面板複製認證 [Marketo的Sales Insight管理頁面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} 並貼到「Salesforce Sales Insight設定」頁面的Rest API區段。

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

就是這樣！ 您應該能夠看到Leads、Contact、Accounts和Opportunity的Marketo Sales Insight欄位。

>[!NOTE]
>
>如果診斷測試失敗，您可能需要 [新增更多欄位至您的頁面配置](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>對於帳戶，銷售分析將包含所有電子郵件，但只有最近有趣的時刻、網頁活動和分數變更。

>[!MORELIKETHIS]
>
>* [優先順序、緊急程度、相對分數和最佳比對](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [將Marketo索引標籤新增至Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [將銷售分析存取權新增至設定檔](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
