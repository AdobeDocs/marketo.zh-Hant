---
unique-page-id: 2360364
description: 第2步（共3步） — 為Marketo建立Salesforce使用者（企業版/不限數量） — Marketo檔案 — 產品檔案
title: 第2步（共3步） — 建立Marketo的Salesforce使用者（企業版/不限數量）
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 2%

---

# 第2步（共3步）:建立Marketo的Salesforce使用者（企業版/無限製版） {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成

>[!PREREQUISITES]
>
>[第1步（共3步）:將Marketo欄位新增至Salesforce（企業版/無限製版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

在本文中，您將在Salesforce設定檔中設定使用者權限，並建立Marketo-Salesforce整合帳戶。

## 建立設定檔 {#create-a-profile}

1. 按一下 **設定**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. 在導覽列中輸入「設定檔」，然後按一下 **設定檔** 連結。

   ![](assets/sfdc-profiles-hands.png)

1. 按一下 **新增**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. 選擇 **標準使用者**，將設定檔命名為「Marketo-Salesforce同步」，然後按一下 **儲存**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## 設定設定檔權限 {#set-profile-permissions}

1. 按一下 **編輯** 來設定安全權限。

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. 在 **管理權限** 部分，確保選中以下框：

   * 啟用API
   * 編輯HTML範本
   * 管理公開文檔
   * 管理公用範本

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >務必檢查 **密碼永不過期** 框。

1. 在「一般使用者權限」區段下，確認已勾選下列方塊：

   * 轉換銷售機會
   * 編輯事件
   * 編輯任務

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. 在「標準對象權限」部分下，確保選中了讀取、建立、編輯和刪除權限：

   * 帳戶
   * 行銷活動
   * 聯繫人
   * 銷售機會
   * 機會

   >[!NOTE]
   >
   >如果您打算使用「促銷活動同步」，請授予「促銷活動」權限。

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. 完成後，按一下 **儲存** 頁面底部。

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## 設定欄位權限 {#set-field-permissions}

1. 與行銷人員討論，了解同步所需的自訂欄位。

   >[!NOTE]
   >
   >此步驟將防止Marketo中顯示您不需要的欄位，以減少雜訊並加速同步。

1. 在設定檔詳細資料頁面中，前往 **欄位層級安全性** 區段。 按一下 **檢視** 要編輯對象的輔助功能，請執行以下操作：

   * 銷售機會
   * 連絡人
   * 帳戶
   * 機會

   >[!TIP]
   >
   >您可以根據組織的需求配置其他對象。

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. 針對每個物件，按一下 **編輯**.

   ![](assets/sfdc-sync-field-edit1.png)

1. 找出不需要的欄位，確定 **讀取存取** 和 **編輯存取** 未勾選。 按一下 **儲存** 等你完事了。

   >[!NOTE]
   >
   >僅編輯自訂欄位的協助工具。

   ![](assets/sfdc-sync-field-edit2.png)

1. 禁用所有不需要的欄位後，必須檢查 **讀取存取和編輯存取** （適用於下列物件欄位）。 按一下 **儲存** 等你完事了。

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
   <td colspan="1" rowspan="1"><p>Event</p></td> 
   <td colspan="1" rowspan="1"><p>所有欄位</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>任務</p></td> 
   <td colspan="1" rowspan="1"><p>所有欄位</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## 建立Marketo-Salesforce同步帳戶 {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>建立專用的Salesforce帳戶(例如marketo@yourcompany.com)，以區分Marketo和其他Salesforce使用者所做的變更。

1. 在導覽列中輸入「管理使用者」，然後按一下 **使用者**. 按一下 **新用戶**.

   ![](assets/sfdc-new-users.png)

1. 填寫必填欄位。 然後，選取 **用戶許可：Salesforce** 和您先前建立的設定檔。 按一下 **儲存** 等你完事了。

   ![](assets/image2014-12-9-9-3a20-3a56.png)

已完成第2步（共2步）。

>[!NOTE]
>
>[第3步（共3步）:Connect Marketo和Salesforce（企業版/無限製版）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
