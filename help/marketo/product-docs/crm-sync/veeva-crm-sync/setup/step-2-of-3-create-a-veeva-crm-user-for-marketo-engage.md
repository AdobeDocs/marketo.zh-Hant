---
description: 第2步（共3步） — 為Marketo Engage建立Veva CRM使用者 — Marketo檔案 — 產品檔案
title: 第2步（共3步） — 為Marketo Engage建立Veva CRM使用者
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 4%

---

# 第2步（共3步）:建立Veva CRM使用者以進行Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>本文中的步驟必須由Veva CRM管理員完成。

>[!PREREQUISITES]
>
>[第1步（共3步）:將Marketo欄位添加到Salesforce(Professional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target=&quot;_blank&quot;}

在本文中，您將使用Veva CRM頁面配置來自訂欄位權限，並建立Marketo-Veva CRM同步使用者。

## 設定頁面配置 {#set-page-layouts}

依照這些步驟操作，Marketo同步使用者便可更新自訂欄位。

1. 按一下導航搜索欄中的「帳戶」（人員帳戶）頁面佈局，而不按Enter鍵，然後按一下「聯繫人」下的「頁面佈局」。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. 按一下 **頁面配置**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. 按一下 **HCP — 專業**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. 按一下並拖曳新 **區段** 到頁面配置中。

1. 輸入&quot;Marketo&quot;作為節名，然後按一下 **確定**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. 按一下「分數」欄位並拖曳至Marketo區段。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. 對下列欄位重複上述步驟：

   * 推斷的城市
   * 推斷公司
   * 推斷國家
   * 推斷的大都會區
   * 推斷的電話區碼
   * 推斷的郵遞區號
   * 推斷的州別地區

   >[!NOTE]
   >
   >這些欄位必須位於頁面版面上，Marketo才能讀/寫這些欄位。

   >[!TIP]
   >
   >向下拖曳至頁面右側，為欄位建立兩欄。 您可以將欄位從一側移至另一側，以平衡欄長度。

1. 完成HCP-Professional佈局後，按一下 **儲存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

>[!NOTE]
>
>對其他「帳戶頁面配置」重複此操作。

## 建立設定檔 {#create-a-profile}

1. 按一下 **設定**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. 在導覽列中輸入「設定檔」，然後按一下 **設定檔** 連結。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. 按一下 **新增**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. 選擇「標準用戶」，將配置檔案命名為「Marketo-Salesforce同步」，然後按一下 **儲存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## 設定設定檔權限 {#set-profile-permissions}

1. 按一下 **編輯** 來設定安全權限。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. 在「管理權限」區段下，確認已選取「已啟用API」。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >請務必勾選「密碼永不過期」方塊。

1. 在「一般使用者權限」區段下，確定已選取「編輯事件」和「編輯工作」。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. 在「標準對象權限」部分下，確保已為帳戶和聯繫人檢查讀取、建立、編輯和刪除權限。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. 在「自訂物件權限」區段下，確定已勾選「讀取」權限，以取得呼叫、呼叫金鑰訊息和任何其他需要的自訂物件。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. 完成後，按一下 **儲存** 頁面底部。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## 設定欄位權限 {#set-field-permissions}

1. 與行銷人員討論，了解同步所需的自訂欄位。

>[!NOTE]
>
>此步驟將防止Marketo中顯示您不需要的欄位，以減少雜訊並加速同步。

1. 在設定檔詳細資訊頁面中，前往欄位層級安全性區段。 按一下「查看」可編輯聯繫人和帳戶對象的輔助功能。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

>[!TIP]
>
>您可以根據組織的需求配置其他對象。

1. 針對每個物件，按一下 **編輯**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

找出不必要的欄位，確定「讀取存取」和「編輯存取」為 **un**&#x200B;已勾選。 按一下 **儲存** 時才能使用。

![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

>[!NOTE]
>
>僅編輯自訂欄位的協助工具。

1. 禁用所有不必要的欄位後，請選中以下對象欄位的「讀取訪問」和「編輯訪問」。 完成後，按一下「儲存」 。

<table>
 <tbody>
  <tr>
   <th>物件
   <th>欄位
  </tr>
  <tr>
   <td>帳戶</td>
   <td>類型欄位</td>
  </tr>
  <tr>
   <td>Event</td>
   <td>所有欄位</td>
  </tr>
  <tr>
   <td>任務</td>
   <td>所有欄位</td>
  </tr>
 </tbody>
</table>

## 建立同步用戶 {#create-sync-user}

Marketo需要憑證才能存取Veva CRM。 使用下列步驟建立的專用使用者，最好能完成此操作。

>[!NOTE]
>
>如果您的組織沒有其他Veva CRM授權，您可以使用具有系統管理員設定檔的現有行銷使用者。

1. 在導覽列中輸入「使用者」，然後按一下 **使用者** 在「管理使用者」下。

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. 按一下 **新用戶**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. 填寫必填欄位，選取「使用者授權」 :Salesforce，設定Profile:Marketo同步使用者，然後按一下 **儲存**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>請確定您輸入的電子郵件地址有效。 您需要以同步使用者身分登入，才能重設密碼。

太棒了！ 現在您有一個帳戶，Marketo Engage可使用該帳戶連線至Veeva CRM。 我們做吧。

>[!MORELIKETHIS]
>
>[第3步（共3步）:連接Marketo和Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target=&quot;_blank&quot;}
