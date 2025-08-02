---
unique-page-id: 2360364
description: 步驟3之2 — 建立Marketo的Salesforce使用者(Enterprise/Unlimited) - Marketo檔案 — 產品檔案
title: 步驟3之2 — 建立Marketo的Salesforce使用者(Enterprise/Unlimited)
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 2%

---

# 步驟2之3：建立Marketo (Enterprise/Unlimited)的[!DNL Salesforce]使用者 {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>這些步驟必須由[!DNL Salesforce]管理員完成

>[!PREREQUISITES]
>
>[步驟3之1：將Marketo欄位新增至 [!DNL Salesforce]  (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

在本文中，您將會在[!DNL Salesforce]設定檔中設定使用者許可權，並建立Marketo-[!DNL Salesforce]整合帳戶。

## 建立設定檔 {#create-a-profile}

1. 按一下「**[!UICONTROL Setup]**」。

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. 在導覽搜尋列中輸入「設定檔」並按一下&#x200B;**[!UICONTROL Profiles]**&#x200B;連結。

   ![](assets/sfdc-profiles-hands.png)

1. 按一下&#x200B;**[!UICONTROL New]**。

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. 選取&#x200B;**[!UICONTROL Standard User]**，將設定檔命名為「Marketo-Salesforce Sync」並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## 設定設定檔許可權 {#set-profile-permissions}

1. 按一下&#x200B;**[!UICONTROL Edit]**&#x200B;以設定安全性許可權。

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. 在&#x200B;**[!UICONTROL Administrative Permissions]**&#x200B;區段下，確定已勾選下列方塊：

   * [!UICONTROL API Enabled]
   * [!UICONTROL Edit HTML Templates]
   * [!UICONTROL Manage Public Documents]
   * [!UICONTROL Manage Public Templates]

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >請務必勾選&#x200B;**[!UICONTROL Password Never Expires]**&#x200B;方塊。

1. 在[!UICONTROL General User Permissions]區段下，確定已勾選下列方塊：

   * [!UICONTROL Convert Leads]
   * [!UICONTROL Edit Events]
   * [!UICONTROL Edit Tasks]

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. 在[!UICONTROL Standard Object Permissions]區段下，確定已檢查[!UICONTROL Read, Create, Edit, and Delete]許可權：

   * [!UICONTROL Accounts]
   * [!UICONTROL Campaigns]
   * [!UICONTROL Contacts]
   * [!UICONTROL Leads]
   * [!UICONTROL Opportunities]

   >[!NOTE]
   >
   >如果您打算使用Campaign Sync，請授與[!UICONTROL Campaigns]的許可權。

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. 完成後，按一下頁面底部的&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## 設定欄位許可權 {#set-field-permissions}

1. 與您的行銷人員討論，找出同步所需的自訂欄位。

   >[!NOTE]
   >
   >此步驟將防止您不需要的欄位顯示在Marketo中，這將減少雜亂並加快同步速度。

1. 在設定檔詳細資訊頁面中，移至&#x200B;**[!UICONTROL Field-Level Security]**&#x200B;區段。 按一下&#x200B;**[!UICONTROL View]**&#x200B;以編輯物件的協助工具：

   * [!UICONTROL Lead]
   * [!UICONTROL Contact]
   * [!UICONTROL Account]
   * [!UICONTROL Opportunity]

   >[!TIP]
   >
   >您可以根據組織的需求設定其他物件。

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. 按一下每個物件的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/sfdc-sync-field-edit1.png)

1. 找到不需要的欄位，確定未勾選&#x200B;**[!UICONTROL Read Access]**&#x200B;和&#x200B;**[!UICONTROL Edit Access]**。 完成時，按一下「**[!UICONTROL Save]**」。

   >[!NOTE]
   >
   >僅編輯自訂欄位的協助工具。

   ![](assets/sfdc-sync-field-edit2.png)

1. 在您停用完所有不需要的欄位後，必須檢查&#x200B;**[!UICONTROL Read Access and Edit Access]**&#x200B;下列物件欄位。 完成時，按一下「**[!UICONTROL Save]**」。

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
>建立專用的[!DNL Salesforce]帳戶(例如，marketo@yourcompany.com)，以區分Marketo與其他[!DNL Salesforce]使用者所做的變更。

1. 在導覽搜尋列中輸入[管理使用者]，然後按一下&#x200B;**[!UICONTROL Users]**。 按一下&#x200B;**[!UICONTROL New User]**。

   ![](assets/sfdc-new-users.png)

1. 填寫必填欄位。 然後，選取&#x200B;**[!UICONTROL User License: Salesforce]**&#x200B;和您先前建立的設定檔。 完成時，按一下「**[!UICONTROL Save]**」。

   ![](assets/image2014-12-9-9-3a20-3a56.png)

步驟3之2已完成。

>[!NOTE]
>
>[步驟3之3：連線Marketo和 [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
