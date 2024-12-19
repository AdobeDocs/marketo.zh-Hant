---
unique-page-id: 2360364
description: 步驟3之2 — 建立Marketo的Salesforce使用者(Enterprise/Unlimited) - Marketo檔案 — 產品檔案
title: 步驟3之2 — 建立Marketo的Salesforce使用者(Enterprise/Unlimited)
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 3%

---

# 步驟2之3：建立Marketo的Salesforce使用者(Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成

>[!PREREQUISITES]
>
>[步驟3之1：將Marketo欄位新增至Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

在本文中，您將會在Salesforce設定檔中設定使用者許可權，並建立Marketo-Salesforce整合帳戶。

## 建立設定檔 {#create-a-profile}

1. 按一下&#x200B;**[!UICONTROL 設定]**。

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. 在導覽搜尋列中輸入「設定檔」，然後按一下&#x200B;**[!UICONTROL 設定檔]**&#x200B;連結。

   ![](assets/sfdc-profiles-hands.png)

1. 按一下&#x200B;**[!UICONTROL 新增]**。

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. 選取&#x200B;**[!UICONTROL 標準使用者]**，將設定檔命名為「Marketo-Salesforce Sync」，然後按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## 設定設定檔許可權 {#set-profile-permissions}

1. 按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;以設定安全性許可權。

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. 在&#x200B;**[!UICONTROL 管理許可權]**&#x200B;區段下，確定已核取下列方塊：

   * API已啟用
   * 編輯HTML範本
   * 管理公開檔案
   * 管理公開範本

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >請務必勾選&#x200B;**[!UICONTROL 密碼永不過期]**&#x200B;方塊。

1. 在「一般使用者許可權」區段下，確定已勾選下列方塊：

   * 轉換潛在客戶
   * 編輯事件
   * 編輯任務

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. 在「標準物件許可權」區段下，確定已勾選「讀取」、「建立」、「編輯」和「刪除」許可權：

   * 帳戶
   * 行銷活動
   * 連絡人
   * 銷售機會
   * 機會

   >[!NOTE]
   >
   >如果您打算使用Campaign Sync，請授與Campaigns的許可權。

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. 完成時，請按一下頁面底部的&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## 設定欄位許可權 {#set-field-permissions}

1. 與您的行銷人員討論，找出同步所需的自訂欄位。

   >[!NOTE]
   >
   >此步驟將防止您不需要的欄位顯示在Marketo中，這將減少雜亂並加快同步速度。

1. 在設定檔詳細資訊頁面中，移至&#x200B;**[!UICONTROL 欄位層級安全性]**&#x200B;區段。 按一下&#x200B;**[!UICONTROL 檢視]**&#x200B;以編輯物件的協助工具：

   * 銷售機會
   * 連絡人
   * 帳戶
   * 機會

   >[!TIP]
   >
   >您可以根據組織的需求設定其他物件。

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. 按一下每個物件的&#x200B;**[!UICONTROL 編輯]**。

   ![](assets/sfdc-sync-field-edit1.png)

1. 找出不需要的欄位，確定已取消勾選&#x200B;**[!UICONTROL 讀取存取權]**&#x200B;和&#x200B;**[!UICONTROL 編輯存取權]**。 完成時，按一下&#x200B;**[!UICONTROL 儲存]**。

   >[!NOTE]
   >
   >僅編輯自訂欄位的協助工具。

   ![](assets/sfdc-sync-field-edit2.png)

1. 當您停用完所有不需要的欄位後，必須核取&#x200B;**[!UICONTROL 下列物件欄位的[讀取存取權]和[編輯存取權]]**。 完成時，按一下&#x200B;**[!UICONTROL 儲存]**。

<table> 
 <tbody> 
  <tr> 
   <th>物件</th> 
   <th>欄位</th> 
  </tr> 
  <tr> 
   <td>帳戶</td> 
   <td>型別欄位</td> 
  </tr> 
  <tr> 
   <td>活動</td> 
   <td>所有欄位</td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>所有欄位</td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## 建立Marketo-Salesforce同步帳戶 {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>建立專用的Salesforce帳戶（例如`marketo@yourcompany.com`），以區分Marketo與其他Salesforce使用者所做的變更。

1. 在導覽搜尋列中輸入[管理使用者]，然後按一下&#x200B;**[!UICONTROL 使用者]**。 按一下&#x200B;**[!UICONTROL 新增使用者]**。

   ![](assets/sfdc-new-users.png)

1. 填寫必填欄位。 接著，選取&#x200B;**[!UICONTROL 使用者授權： Salesforce]**&#x200B;以及您先前建立的設定檔。 完成時，按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/image2014-12-9-9-3a20-3a56.png)

步驟3之2已完成。

>[!NOTE]
>
>[步驟3之3：連線Marketo和Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}
