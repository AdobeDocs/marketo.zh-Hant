---
unique-page-id: 3571743
description: 在Salesforce專業版中設定Marketo Sales Insight - Marketo Docs —— 產品檔案
title: 在Salesforce Professional Edition中設定Marketo Sales Insight
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---


# 在Salesforce Professional Edition中設定Marketo Sales Insight {#configure-marketo-sales-insight-in-salesforce-professional-edition}

以下是在Salesforce Professional Edition中設定Marketo Sales Insight時需要採取的步驟。 我們開始吧。

>[!PREREQUISITES]
>
>* 在您的Salesforce Professional Edition中安裝Marketo。
   >
   >
* [在Salesforce AppExchange中安裝Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
>
>**需要管理員權限**

## 在Marketon中設定Sales Insight {#configure-sales-insight-in-marketo}

1. 開啟新的瀏覽器視窗，從您的Marketo帳戶取得Marketo Sales Insight認證。
1. 前往「管理員」區域並選取「銷售分析」**。**

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. 按一下「編輯API設定」。****

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. 輸入您選擇的API密鑰，然後按一下&#x200B;**保存**。 請勿在API密鑰中使用&amp;符號。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >您的API密鑰就像組織的密碼，應該是安全的。

1. 按一下「Rest API設定」面板中的「檢視」****，以填入憑證。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. 您會看到確認快顯視窗。 按一下&#x200B;**確定**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## 在Salesforce {#configure-sales-insight-in-salesforce}中設定Sales Insight

1. 在Salesforce中，按一下「**Setup**」。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. 搜索「遠程站點」並選擇「**遠程站點設定」**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. 按一下&#x200B;**新建遠程站點**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. 輸入遠端網站名稱（可以是類似「MarketoSoapAPI」的名稱）。 從Marketo的「Soap API設定」面板輸入遠端網站URL，此為您的Marketo主機URL。 按一下&#x200B;**保存**。 您現在已建立Soap API的遠端網站設定。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. 再次按一下&#x200B;**新建遠程站點**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. 輸入遠端網站名稱（可以是類似「MarketoRestAPI」的名稱）。 輸入遠端網站URL，此為Marketo中「Rest API設定」面板的API URL。 按一下&#x200B;**保存**。 您現在已建立Rest API的遠端網站設定。

## 設定Marketo Sales Insight {#set-up-marketo-sales-insight}

1. 登入您的Marketo例項，然後按一下&#x200B;**管理**。

   ![](assets/login-admin-1.png)

1. 按一下&#x200B;**Sales Insight**。

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. 按一下「編輯API設定」。****

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. 輸入&#x200B;**API密鑰**，然後按一下&#x200B;**保存**。

   >[!CAUTION]
   >
   >請勿在API密鑰中使用&amp;符號。

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >把窗子開啟。 您稍後在Salesforce中將需要此資訊。

1. 返回Salesforce，按一下「設定」。****

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 搜索「遠程站點」，然後按一下&#x200B;**安全控制**&#x200B;下的&#x200B;**遠程站點設定**。

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. 按一下&#x200B;**新建遠程站點**。

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. 輸入&#x200B;**遠程站點名稱**&#x200B;和&#x200B;**遠程站點URL**，然後按一下&#x200B;**保存**。

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >您可選擇&#x200B;**遠端網站名稱**（此處使用MarketoAPI）。 在步驟4的「編輯API設定」對話方塊的「行銷人員主機」欄位中，可找到&#x200B;**遠端網站URL**。

## 自訂頁面版面{#customize-page-layouts}

1. 按一下&#x200B;**Setup**。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 搜索「頁面佈局」並選擇&#x200B;**Leads**&#x200B;下的&#x200B;**頁面佈局**。

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. 按一下左側的&#x200B;**Visualforce Pages**。 將&#x200B;**Section**&#x200B;拖曳至「自訂連結」區段下的版面。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 輸入「Marketo Sales Insight」作為&#x200B;**區段名稱**。 選擇&#x200B;**1-Column**&#x200B;並按一下&#x200B;**確定**。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 將&#x200B;**Lead**&#x200B;拖放到新區段中。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此框的名稱將根據對象類型而更改。 例如，如果您要修改Contacts的頁面佈局，則會顯示Contact。

1. 按兩下剛添加的&#x200B;**Lead**&#x200B;塊。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 將高度編輯為&#x200B;**450**&#x200B;像素，然後按一下&#x200B;**確定**。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >我們建議Accounts和Opportunity物件的高度為410像素。

1. 按一下左側的&#x200B;**欄位**。 然後搜尋並拖曳&#x200B;**Engagement**&#x200B;標籤至&#x200B;**Marketo Sales Insight**&#x200B;版面。

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

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

1. 完成後，按一下&#x200B;**保存**。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重複此過程，為&#x200B;**Contact**、**Account**&#x200B;和&#x200B;**Opportunity**&#x200B;添加Visualforce頁面部分和Sales Insight欄位。
1. 重複步驟5-7，為Contact 、 Account和Opportunity添加Visualforce頁面部分。 然後，重複步驟8-10，為&#x200B;**Contact**&#x200B;添加Sales Insight欄位。 請務必在變更後儲存。

## 映射自定義人員欄位{#map-custom-person-fields}

行銷人員欄位必須對應至Salesforce連絡人欄位，以確保轉換正常運作。 這是方法。

1. 按一下&#x200B;**Setup**。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 在搜索欄中搜索「欄位」，然後按一下&#x200B;**Leads**&#x200B;下的&#x200B;**Fields**。

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. 按一下&#x200B;**映射銷售線索欄位**。

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. 按一下右側的下拉式清單，顯示&#x200B;**Engagement**。

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. 在清單中選擇&#x200B;**Contact.Engagement**。

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

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

1. 完成時，按一下「儲存」。****

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketo Sales Insight設定{#marketo-sales-insight-config}

1. 按一下&#x200B;**+**，然後選取&#x200B;**Marketo Sales Insight Config**。

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. 勾選&#x200B;**啟用Marketo API**。 然後，填寫Marketo Admin](#set-up-marketo-sales-insight)中的[API設定資訊。 完成時，按一下「保存更改」。****

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >如果診斷測試失敗，您可能需要[將更多欄位新增至頁面配置](https://nation.marketo.com/docs/DOC-1115)。

就這樣！ 您應該能夠查看Lead 、 Contacts 、 Accounts和Opportunity的Marketo Sales Insight欄位。

![](assets/twenty-six-1.png)

>[!NOTE]
>
>對於帳戶，Sales Insight將包含所有電子郵件，但僅包含最新的有趣時刻、網頁活動和分數變更。

## 存取Marketor Sales Insight {#access-marketo-sales-insight}

1. 在Salesforce中，按一下標籤列結尾的&#x200B;**+**，然後按一下「Marketo Sales Insight設定」。****

1. 選取&#x200B;**啟用Marketo API**&#x200B;核取方塊。

1. 從Marketo的「銷售分析管理」頁面的「Soap API」面板複製認證，並貼到「Salesforce銷售分析設定」頁面的「Soap API」區段中。

1. 從Marketo的「銷售分析管理」頁面的「Rest API」面板複製認證，並貼到「Salesforce Sales Insight設定」頁面的「Rest API」區段中。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

>[!MORELIKETHIS]
>
>* [優先順序、緊急程度、相對分數和最佳賭注](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [新增Market至Sales Insight標籤和按鈕至Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)

