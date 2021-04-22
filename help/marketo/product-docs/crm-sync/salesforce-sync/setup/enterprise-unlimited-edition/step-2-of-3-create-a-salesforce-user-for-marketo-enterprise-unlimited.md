---
unique-page-id: 2360364
description: 第2步（共3步）-建立適用於Marketo的Salesforce使用者（企業版／不限數量）-Marketo檔案——產品檔案
title: 第2步（共3步）-建立適用於Marketo的Salesforce使用者（企業版／無限製版）
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# 步驟2（共3步）:為Marketo建立Salesforce使用者（企業版／無限製版）{#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成

>[!PREREQUISITES]
>
>[步驟1（共3步）:將Marketo欄位新增至Salesforce（企業版／無限製版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

在本文中，您將在Salesforce設定檔中設定使用者權限，並建立Marketo-Salesforce整合帳戶。

## 建立配置檔案{#create-a-profile}

1. 按一下&#x200B;**Setup**。

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. 在Nav搜索欄中鍵入&quot;profiles&quot;，然後按一下&#x200B;**Profiles**&#x200B;連結。

   ![](assets/sfdc-profiles-hands.png)

1. 按一下&#x200B;**新建**。

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. 選擇「**標準用戶**」，將配置檔案命名為「Marketo-Salesforce同步」，然後按一下「保存」。****

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## 設定描述檔權限{#set-profile-permissions}

1. 按一下&#x200B;**編輯**&#x200B;以設定安全權限。

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. 在&#x200B;**管理權限**&#x200B;區段下，請確定已勾選下列方塊：

   * 啟用API
   * 編輯HTML範本
   * 管理公開檔案
   * 管理公用範本

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >請務必選中&#x200B;**密碼永不過期**&#x200B;框。

1. 在「一般使用者權限」區段下，請確定已勾選下列方塊：

   * 轉換銷售線索
   * 編輯事件
   * 編輯任務

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. 在「標準物件權限」區段下，請確定已勾選「讀取」、「建立」、「編輯」和「刪除」權限：

   * 帳戶
   * 促銷活動
   * 聯絡人
   * 銷售線索
   * 機會

   >[!NOTE]
   >
   >如果您打算使用「促銷活動同步」，請授予「促銷活動」權限。

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. 完成後，按一下頁面底部的&#x200B;**Save**。

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## 設定欄位權限{#set-field-permissions}

1. 與行銷人員討論，以瞭解同步所需的自訂欄位。

   >[!NOTE]
   >
   >此步驟可防止您不需要的欄位在Marketo顯示，如此可減少雜亂並加速同步。

1. 在描述檔詳細資訊頁面中，前往&#x200B;**Field-Level Security**&#x200B;區段。 按一下&#x200B;**View**&#x200B;可編輯對象的輔助功能：

   * 銷售線索
   * 聯絡人
   * 帳戶
   * 機會

   >[!TIP]
   >
   >您可以根據組織的需要配置其他對象。

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. 對於每個對象，按一下&#x200B;**編輯**。

   ![](assets/sfdc-sync-field-edit1.png)

1. 找到不需要的欄位，確保&#x200B;**讀訪問**&#x200B;和&#x200B;**編輯訪問**&#x200B;未選中。 完成時，按一下「儲存」。****

   >[!NOTE]
   >
   >僅編輯自訂欄位的協助功能。

   ![](assets/sfdc-sync-field-edit2.png)

1. 在禁用所有不需要的欄位後，必須選中&#x200B;**讀取訪問和編輯訪問**&#x200B;以查看以下對象欄位。 完成時，按一下「儲存」。****

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>物件</p></th> 
   <th colspan="1" rowspan="1"><p>欄位</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>帳戶</p></td> 
   <td colspan="1" rowspan="1"><p>類型欄位</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>事件</p></td> 
   <td colspan="1" rowspan="1"><p>所有欄位</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>任務</p></td> 
   <td colspan="1" rowspan="1"><p>所有欄位</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## 建立Marketo-Salesforce同步帳戶{#create-marketo-salesforce-sync-account}

>[!TIP]
>
>建立專屬的Salesforce帳戶(例如marketo@yourcompany.com)，以區分Marketo和其他Salesforce使用者所做的變更。

1. 在導覽列中輸入「管理使用者」，然後按一下「**使用者**」。 按一下&#x200B;**New User**。

   ![](assets/sfdc-new-users.png)

1. 填寫必填欄位。 然後，選擇&#x200B;**用戶許可證：Salesforce**&#x200B;和您先前建立的設定檔。 完成時，按一下「儲存」。****

   ![](assets/image2014-12-9-9-3a20-3a56.png)

步驟2（共2步）已完成。

>[!NOTE]
>
>[步驟3（共3步）:連接Marketo和Salesforce（企業版／無限製版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
