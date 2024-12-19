---
unique-page-id: 2360362
description: 步驟3之1 — 將Marketo欄位新增至Salesforce (Enterprise/Unlimited) - Marketo檔案 — 產品檔案
title: 步驟3之1 — 將Marketo欄位新增至Salesforce (Enterprise/Unlimited)
exl-id: bcfba281-0d4b-42c3-b52a-ce1c3da884ba
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 7%

---

# 步驟3之1：將Marketo欄位新增至Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>您必須有權存取Salesforce API，才能在Marketo Engage與Salesforce之間同步。

Marketo使用一組欄位來擷取特定型別的行銷相關資訊。 如果您想在Salesforce中使用此資料，請遵循下列指示。

1. 在潛在客戶和聯絡物件的Salesforce中建立三個自訂欄位：分數、贏取方案和贏取日期。
1. 在潛在客戶與聯絡人之間對應這些自訂欄位，以便在Salesforce中進行轉換時值能延續。
1. 如有需要，您可以建立其他欄位（請參閱下表）。

所有這些自訂欄位都是選用欄位，不需要用來同步Marketo和Salesforce。 根據最佳實務，建議您建立「分數」、「贏取方案」和「贏取日期」欄位。

## 將Marketo欄位新增至Salesforce {#add-marketo-fields-to-salesforce}

在以上列出的Salesforce中的潛在客戶與聯絡人物件上，新增三個自訂欄位。 如果您想要新增更多欄位，請參閱本區段末尾的可用欄位表。

對三個自訂欄位中的每一個執行以下步驟以新增它們。 從分數開始。

1. 登入Salesforce並按一下&#x200B;**[!UICONTROL 設定]**。

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. 在左側的[!UICONTROL 建置]功能表中，按一下&#x200B;**[!UICONTROL 自訂]**&#x200B;並選取&#x200B;**[!UICONTROL 銷售機會]**。 按一下&#x200B;**[!UICONTROL 欄位]**。

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. 在頁面底部的[自訂欄位和關聯性]區段中，按一下&#x200B;**[!UICONTROL 新增]**。

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. 選擇適當的欄位型別（「分數 — 數字」、「贏取方案 — 文字」、「贏取日期 — 日期/時間」）。

   ![](assets/choose-field-type-2-hand.png)

1. 按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. 輸入欄位的[!UICONTROL 欄位標籤]、[!UICONTROL 長度]和[!UICONTROL 欄位名稱]，如下表所示。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      欄位標籤 
    </div></th> 
   <th> 
    <div>
      欄位名稱 
    </div></th> 
   <th> 
    <div>
      資料類型 
    </div></th> 
   <th> 
    <div>
      欄位屬性 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>分數</td> 
   <td>mkto71_Lead_Score</td> 
   <td>數字</td> 
   <td>長度10<br>小數位數0 </td> 
  </tr> 
  <tr> 
   <td>獲取日期</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>日期/時間</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>贏取方案</td> 
   <td>mkto71_Acquisition_Program</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Salesforce在用來建立API名稱時，會將__c附加至欄位名稱。

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>文字和數字欄位需要長度，但日期/時間欄位不需要。說明為選用。

1. 按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. 指定存取設定，然後按一下&#x200B;**[!UICONTROL 下一步]**：

   * 將所有角色設定為&#x200B;**[!UICONTROL 可見]**&#x200B;和&#x200B;**[!UICONTROL 唯讀]**

   * 清除同步處理使用者設定檔的&#x200B;**[!UICONTROL 唯讀]**&#x200B;核取方塊：

      * 如果您的使用者具有&#x200B;_系統管理員_&#x200B;的設定檔作為同步使用者，請清除系統管理員設定檔的&#x200B;**[!UICONTROL 唯讀]**&#x200B;核取方塊（如下所示）
      * 如果您已建立同步處理使用者的&#x200B;_自訂設定檔_，請清除該自訂設定檔的&#x200B;**[!UICONTROL 唯讀]**&#x200B;核取方塊

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. 選擇應顯示欄位的頁面配置。

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. 按一下[儲存與新增]****，返回並建立其他兩個自訂欄位。 完成全部三個動作後，按一下[儲存]。****

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. 在左側的[組建]功能表中，按一下[自訂] ****，然後選取[連絡人]。 按一下「欄位」。
1. 針對連絡人物件的「分數」、「贏取日期」和「贏取方案」欄位，執行步驟3到10，就像您對潛在客戶物件所做的一樣。
1. 或者，您可以將此程式用於此表格的任何其他自訂欄位。

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      欄位標籤 
    </div></th> 
   <th> 
    <div>
      欄位名稱 
    </div></th> 
   <th> 
    <div>
      資料類型 
    </div></th> 
   <th> 
    <div>
      欄位屬性 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>贏取方案ID</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>數字</td> 
   <td>長度18<br>小數位數0 </td> 
  </tr> 
  <tr> 
   <td>原始反向連結</td> 
   <td>mkto71_Original_Referrer</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>原始搜尋引擎</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>原始搜尋片語</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>原始來源資訊</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>原始來源類型</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>推斷的城市</td> 
   <td>mkto71_Inferred_City</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>推斷的公司</td> 
   <td>mkto71_Inferred_Company</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>推斷的國家</td> 
   <td>mkto71_Inferred_Country</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>推斷的大都會區</td> 
   <td>mkto71_Inferred_Metropolitan_Area</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>推斷的電話區碼</td> 
   <td>mkto71_Inferred_Phone_Area_Code</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>推斷的郵遞區號</td> 
   <td>mkto71_Inferred_Postal_Code</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
  <tr> 
   <td>推斷的州別區域</td> 
   <td>mkto71_Inferred_State_Region</td> 
   <td>文字</td> 
   <td>長度255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>建立新欄位後，Marketo自動指派的欄位值將無法立即在Salesforce中使用。 下次更新任一系統上的記錄時(即更新任何在Salesforce和Marketo之間同步的欄位)，Marketo會將資料同步至Salesforce。

## 對應自訂欄位以進行轉換 {#map-custom-fields-for-conversions}

Salesforce中潛在客戶物件上的自訂欄位應對應至聯絡人物件上的聯絡人欄位，以便在轉換發生時保留資料。

1. 按一下右上角的&#x200B;**[!UICONTROL 設定]**。

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. 在導覽搜尋中輸入「欄位」，不按Enter鍵。 欄位會顯示在不同的物件下；按一下[潛在客戶]下的&#x200B;**[!UICONTROL 欄位]**。

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. 移至[潛在客戶自訂欄位與關係]區段，然後按一下[對映潛在客戶欄位] ]**。**[!UICONTROL 

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. 按一下您要對應的欄位旁邊的下拉式清單。

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. 選取對應的連絡人自訂欄位。

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. 對您已建立的任何其他欄位重複上述步驟。

1. 完成時，按一下&#x200B;**[!UICONTROL 儲存]**。

>[!MORELIKETHIS]
>
>[步驟2之3：建立Marketo (Enterprise/Unlimited)的Salesforce使用者](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
