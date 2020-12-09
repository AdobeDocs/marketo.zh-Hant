---
unique-page-id: 2360364
description: 第2步（共3步）-建立適用於行銷人員的Salesforce使用者（企業版／不限數量）-行銷人員檔案——產品檔案
title: 第2步（共3步）-建立適用於行銷人員的Salesforce使用者（企業版／不限數量）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# 步驟2（共3步）:建立適用於行銷人員的Salesforce使用者（企業版／不限數量） {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>這些步驟必須由Salesforce管理員完成

>[!PREREQUISITES]
>
>* [步驟1（共3步）:將行銷人員欄位新增至Salesforce（企業版／無限製版）](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

>



在本文中，您將在Salesforce設定檔中設定使用者權限，並建立Marketo-Salesforce整合帳戶。

## 建立描述檔 {#create-a-profile}

1. 按一 **下設定**。

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. 在導覽搜尋列中輸入「描述檔」，然後按一下「描述檔 **」連結** 。

   ![](assets/sfdc-profiles-hands.png)

1. 按一下「 **新增**」。

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. 選取「 **標準使用者**」，將描述檔命名為「Marketo-Salesforce同步」，然後按一下「 **儲存」**。

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## 設定設定檔權限 {#set-profile-permissions}

1. 按一 **下「編輯** 」以設定安全權限。

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. 在「管 **理權限** 」區段下，請確定已勾選下列方塊：

   * 啟用API
   * 編輯HTML範本
   * 管理公開檔案
   * 管理公用範本

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >請務必勾選「密碼 **永不過期** 」方塊。

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

1. 完成後，按一 **下頁** 面底部的「儲存」。

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## 設定欄位權限 {#set-field-permissions}

1. 與行銷人員討論，以瞭解同步所需的自訂欄位。

   >[!NOTE]
   >
   >此步驟可防止您不需要的欄位在Marketo中顯示，如此可減少雜亂並加速同步。

1. 在描述檔詳細資訊頁面中，前往 **欄位層級安全性區段** 。 按一下 **查看** ，編輯對象的輔助功能：

   * `Lead`
   * `Contact`
   * `Account`
   * `Opportunity`

   >[!TIP]
   >
   >您可以根據組織的需要配置其他對象。

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. 對於每個對象，按一下「編 **輯」**。

   ![](assets/sfdc-sync-field-edit1.png)

1. 找到不需要的欄位，請確定未勾選「**讀取存 **取** 」和「編輯存取」**。 完 **成時** ，按一下「儲存」。

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >僅編輯自訂欄位的協助功能。

   ![](assets/sfdc-sync-field-edit2.png)

1. 在禁用完所有不需要的欄位後，必須選中**讀訪問和編輯訪問**以查看以下對象欄位。 完 **成時** ，按一下「儲存」。

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

## 建立Marketo-Salesforce同步帳戶 {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>建立專屬的Salesforce帳戶(例如 [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#89e4e8fbe2ecfde6c9f0e6fcfbeae6e4f9e8e7f0a7eae6e4))，以區分Marketo和其他Salesforce使用者所做的變更。

1. 在導覽搜尋列中輸入「管理使用者」，然後按一下「使 **用者**」。 按一下「 **新使用者**」。

   ![](assets/sfdc-new-users.png)

1. 填寫必填欄位。 然後，選取「使用 **者授權」:Salesforce** 和您先前建立的設定檔。 完 **成時** ，按一下「儲存」。

   ![](assets/image2014-12-9-9-3a20-3a56.png)

步驟2（共2步）已完成。

>[!NOTE]
>
>**相關文章**
>
>* [步驟3（共3步）:將行銷人員連線至Salesforce（企業版／無限製版）](step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)

>



