---
unique-page-id: 2360368
description: 在Salesforce Enterprise中設定Marketo Sales Insight/Unlimited - Marketo Docs —— 產品檔案
title: 在Salesforce Enterprise中設定Marketo Sales Insight/Unlimited
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---


# 在Salesforce Enterprise中設定Marketo Sales Insight/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

以下是在Salesforce Enterprise/Unlimited Editions中設定Marketo Sales Insight時需要執行的步驟。 我們開始吧。

>[!PREREQUISITES]
>
>* [在您的Salesforce Enterprise/Unlimited Edition中設定Marketo欄位同步](http://docs.marketo.com/pages/viewpage.action?pageid=2360372)
>* [在Salesforce AppExchange中安裝Marketo Sales Insight套件](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>



>[!NOTE]
>
>**需要管理員權限**

## 在Marketo中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 開啟新的瀏覽器視窗，從您的Marketo帳戶取得Marketo Sales Insight認證。
1. 前往「管理員」區域並選取「 **銷售分析」**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 按一 **下編輯API設定**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 輸入您選擇的API密鑰，然後按一下「儲 **存**」。 請勿在API密鑰中使用&amp;符號。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >您的API密鑰就像組織的密碼，應該是安全的。

1. 按一 **下** 「Rest API Configuration」（其餘API設定）面板中的「View」（檢視）以填入憑證。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 您會看到確認快顯視窗。 按一下 **確定**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

## 在Salesforce中設定Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，按一下「 **設定**」。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 搜索「遠程站點」並選擇「 **遠程站點設定」**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 按一下 **新建遠程站點**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. 輸入遠端網站名稱（可以是類似「MarketoSoapAPI」的名稱）。 從Marketo的「Soap API設定」面板輸入遠端網站URL，此為您的Marketo主機URL。 按一下 **儲存**。 您現在已建立Soap API的遠端網站設定。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. 再次 **按一下「新建遠程站點** 」。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. 輸入遠端網站名稱（可以是類似「MarketoRestAPI」的名稱）。 輸入遠端網站URL，此為Marketo中「Rest API設定」面板的API URL。 按一下 **儲存**。 您現在已建立Rest API的遠端網站設定。

## 設定Marketo Sales Insight {#set-up-marketo-sales-insight}

1. 登入您的Marketo例項，然後按一下「管 **理員**」。

   ![](assets/login-admin.png)

1. 按一下** Sales Insight**。

   ![](assets/image2015-5-22-15-3a12-3a33.png)

1. 按一 **下編輯API設定**。

   ![](assets/image2015-5-22-15-3a15-3a0.png)

1. 輸入 **API密鑰** ，然後按 **一下儲存**。

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2015-5-27-16-3a36-3a56.png)

   >[!TIP]
   >
   >把窗子開啟。 您稍後在Salesforce中將需要此資訊。

1. 返回Salesforce，按一下「設 **定」**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 搜索「遠程站點」，然後按一下「 **安全控制」下的** 「遠 **程站點設定」**。

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. 按一下 **新建遠程站點**。

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. 輸入 **遠端網站名稱****和遠端網站URL**，然後按一 **下儲存**。

   ![](assets/remote-site.png)

   >[!NOTE]
   >
   >您選擇您的 **遠端網站名稱** （此處使用MarketoAPI）。 您可 **以在步驟** 4的「編輯API設定」對話方塊的「Marketo Host」欄位中找到「遠端網站URL」。

## 自訂頁面版面 {#customize-page-layouts}

1. 按一 **下設定**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 搜索「頁面佈局」並選擇「銷 **售線索** 」下 **的「頁面佈局」**。

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 按一下左側的**Visualforce頁面**。 將「 **區段** 」拖曳至「自訂連結」區段下的版面。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 輸入「Marketo Sales Insight」作為區 **段名稱**。 選擇 **1-Column** ，然後按一下 **確定**。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 將Lead拖 **放至** 新區段。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此框的名稱將根據對象類型而更改。 例如，如果您要修改Contacts的頁面佈局，則會顯示Contact。

1. 按兩下剛添加 **的** Lead塊。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 編輯高度至 **450像素** ，然後按一下「 **確定」**。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >我們建議Accounts和Opportunity物件的高度為410像素。

1. 按一下左側的**欄位**。 然後搜尋並拖曳 **Engagement** 標籤至 **** Marketo Sales Insight版面。

   ![](assets/image2015-5-22-16-3a32-3a46.png)

1. 對這些欄位重複上述步驟。

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">參與</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>相對分數值</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>緊急值</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後一個有趣的時刻</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後一個有趣的時刻Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後一個有趣的時刻來源</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後一個有趣的力矩類型</p></td> 
  </tr> 
 </tbody> 
</table>

1. 完成後 **按一下** 「儲存」。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重複此程式，以新增Contact、Account和Opportunity的Visualforce頁面區 **段和Sales Insight****欄** 位 ****。
1. 重複步驟5-7，為Contact 、 Account和Opportunity添加Visualforce頁面部分。 然後，重複步驟8-10以新增Contact的Sales Insight欄 **位**。 請務必在變更後儲存。

## 對應自訂人員欄位 {#map-custom-person-fields}

行銷人員欄位必須對應至Salesforce連絡人欄位，以確保轉換正常運作。 這是方法。

1. 按一 **下設定**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 在搜索欄中搜索「欄位」，然後按一下「銷 **售線索** 」下 **的「欄位」**。

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 按一 **下「對應銷售線索欄位**」。

   ** ![](assets/image2015-6-1-9-3a58-3a48.png)

   **

1. 按一下「參與」右側的下拉式 **清單**。

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. 在清單中選取**Contact.Engagement **。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. 重複這些欄位並對應這些欄位。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">行銷人員自訂欄位</th> 
   <th colspan="1" rowspan="1">Salesforce連絡人自訂欄位</th> 
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
   <td colspan="1" rowspan="1"><p>最後一個有趣的時刻</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.最後一個有趣的時刻日期</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後一個有趣的時刻Desc</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Monet Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後一個有趣的時刻來源</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Source</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最後一個有趣的力矩類型</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Type</p></td> 
  </tr> 
 </tbody> 
</table>

1. 完成時，按一下「**儲存**」。

## Marketo Sales Insight設定 {#marketo-sales-insight-config}

1. 按一下**+ **，然後選取「 **Marketo Sales Insight設定」**。

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. 勾選 **啟用Marketo API**。 然後，在Marketo Admin中填 [寫「API設定」資訊](http://docs.marketo.com/display/DOCS/Configure+Marketo+Sales+Insight+in+Salesforce+Professional+Edition#ConfigureMarketoSalesInsightinSalesforceProfessionalEdition-SetupMarketoSalesInsight)。 完成時，按一下「儲存變更」。

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >如果診斷測試失敗，您可能需要將 [更多欄位新增至頁面配置](http://nation.marketo.com/docs/DOC-1115)。

就這樣！ 您應該能夠查看Lead 、 Contacts 、 Accounts和Opportunity的Marketo Sales Insight欄位。

![](assets/twenty-six.png)

>[!NOTE]
>
>對於帳戶，Sales Insight將包含所有電子郵件，但僅包含最新的有趣時刻、網頁活動和分數變更。

## Access Marketto Sales Insight {#access-marketo-sales-insight}

1. 在Salesforce中，按一 **下標籤列結** 尾的+，然後按一下 **Marketo Sales Insight設定**。
1. 選取「啟 **用Marketo API** 」核取方塊。
1. 從Marketo的「銷售分析管理」頁面的「Soap API」面板複製認證，並貼到「Salesforce銷售分析設定」頁面的「Soap API」區段中。
1. 從Marketo的「銷售分析管理」頁面的「Rest API」面板複製認證，並貼到「Salesforce Sales Insight設定」頁面的「Rest API」區段中。

   ![](assets/access-msi.png)

>[!NOTE]
>
>**相關文章**
>
>* [優先順序、緊急程度、相對分數和最佳賭注](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [新增Market至Sales Insight標籤和按鈕至Salesforce](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)

>



