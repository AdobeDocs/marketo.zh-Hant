---
description: 銷售Insight動作管理員設定指南 — Marketo檔案 — 產品檔案
title: 銷售洞察動作管理員設定指南
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 3%

---

# 銷售洞察動作管理員設定指南 {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions是網頁式應用程式，透過[Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}專門與Salesforce CRM整合。 有時稱為「Marketo銷售」，或簡稱為「動作」。

>[!PREREQUISITES]
>
>* 向Adobe帳戶團隊（您的帳戶管理員）確認已為您的Marketo Engage帳戶啟用MSI動作(如果您沒有帳戶管理員，請聯絡[Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"})。
>* 必須設定您的Marketo/Salesforce同步處理。

<table>
 <tr>
  <th>人物誌</th>
  <th>步驟</th>
 </tr>
 <tr>
  <td>Marketo管理員</td>
  <td>設定Marketo銷售帳戶</td>
 </tr>
 <tr>
  <td>Marketo管理員或<br/>[!DNL Salesforce]管理員</td>
  <td>將Marketo Sales帳戶連線至 [!DNL Salesforce]</td>
 </tr>
 <tr>
  <td>Marketo管理員</td>
  <td>將Marketo Sales帳戶連線至Marketo</td>
 </tr>
 <tr>
  <td>Marketo管理員</td>
  <td>啟動從Marketo到Marketo銷售帳戶的資料同步</td>
 </tr>
 <tr>
  <td>Marketo管理員</td>
  <td>邀請使用者加入MSI-Actions</td>
 </tr>
 <tr>
  <td>[!DNL Salesforce] 管理員</td>
  <td>在安裝/升級MSI封裝 [!DNL Salesforce]</td>
 </tr>
 <tr>
  <td>[!DNL Salesforce] 管理員</td>
  <td>在中設定MSI動作 [!DNL Salesforce]</td>
 </tr>
</table>

## 設定Marketo銷售帳戶 {#set-up-marketo-sales-account}

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >如果您在整合資訊卡片上未看到使用者端ID和使用者端密碼，請邀請第一個使用者來啟動您的動作執行個體，然後您就會看到使用者端ID和使用者端密碼出現。

1. 按一下&#x200B;**銷售Insight**，然後按一下&#x200B;**動作設定**。 從要邀請的Marketo管理員清單中選取，然後按一下&#x200B;**傳送邀請**。

   ![](assets/msi-actions-admin-guide-2.png)

使用者會收到電子郵件，其中包含存取帳戶的步驟。

>[!NOTE]
>
>其他使用者將不會透過Marketo新增，而是透過「銷售帳戶使用者管理」頁面新增。 [按一下這裡](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"}以進一步瞭解新增其他使用者。

## 將Marketo銷售帳戶連線至[!DNL Salesforce] {#connect-marketo-sales-account-to-salesforce}

1. 在您的Marketo銷售帳戶中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/msi-actions-admin-guide-3.png)

1. 在[!UICONTROL Admin Settings]底下，按一下&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/msi-actions-admin-guide-4.png)

1. 在[!UICONTROL Connections & Customizations]索引標籤中，按一下&#x200B;**[!UICONTROL Connect]**。

   ![](assets/msi-actions-admin-guide-5.png)

1. 按一下「**[!UICONTROL OK]**」。

   ![](assets/msi-actions-admin-guide-6.png)

如果您已登入Salesforce，即可連線。 否則，系統會要求您登入。

## 將Marketo連線至您的Sales Apps帳戶 {#connect-marketo-to-your-sales-apps-account}

1. 在您的Marketo銷售帳戶中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/msi-actions-admin-guide-7.png)

1. 在[!UICONTROL Admin Settings]底下，按一下&#x200B;**Marketo**。

   ![](assets/msi-actions-admin-guide-8.png)

1. 按一下&#x200B;**[!UICONTROL connect]**。 然後會連線您的帳戶。

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>如果未連線，請從Marketo Sales Insight的「動作設定」標籤複製認證，然後貼到「設定」標籤中。

## 啟動資料同步 {#initiate-data-sync}

Sales Insight Actions的資料統一欄位同步可讓系統從Marketo Engage資料庫將人員資訊提取到Sales Insight Actions資料庫，讓您的人員資料保持最新，並確保活動記錄到Marketo和[!DNL Salesforce]的正確記錄。

>[!CAUTION]
>
>啟動資料同步之後，您應該&#x200B;**不應**&#x200B;移除銷售Insight動作執行個體上的原始使用者。 這是第一個邀請收件者的使用者。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/msi-actions-admin-guide-10.png)

1. 按一下「**[!UICONTROL Sales Insight]**」。

   ![](assets/msi-actions-admin-guide-11.png)

1. 按一下「**[!UICONTROL Actions Config]**」索引標籤。在動作欄位同步卡中，按一下&#x200B;**[!UICONTROL Sync]**。

   ![](assets/msi-actions-admin-guide-12.png)

1. 您會看到即將同步之欄位的預覽。 按一下「**[!UICONTROL Start Sync]**」。

   ![](assets/msi-actions-admin-guide-13.png)

Marketo和[!DNL Salesforce]中存在的個人記錄將同步至您的Marketo銷售應用程式帳戶。

>[!NOTE]
>
>若要進一步瞭解人員與活動資料如何在Sales Insight Actions、Marketo和Salesforce之間同步，[請按一下這裡](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}。

## 邀請個別使用者加入MSI動作 {#invite-individual-users-to-msi-actions}

1. 在您的Marketo銷售帳戶中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/msi-actions-admin-guide-14.png)

1. 在[!UICONTROL Admin Settings]下，選取&#x200B;**[!UICONTROL User Management]**。

   ![](assets/msi-actions-admin-guide-15.png)

1. 按一下&#x200B;**[!UICONTROL Actions]**&#x200B;並選取&#x200B;**[!UICONTROL Invite Users]**。

   ![](assets/msi-actions-admin-guide-16.png)

1. 輸入電子郵件地址並按一下&#x200B;**[!UICONTROL Invite]**。

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>依預設，所有新成員都會新增至「所有人」團隊。

您將會收到確認訊息。

## 透過CSV邀請使用者加入MSI動作 {#invite-users-via-csv-to-msi-actions}

1. 在您的Marketo銷售帳戶中，按一下齒輪圖示並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/msi-actions-admin-guide-18.png)

1. 在[!UICONTROL Admin Settings]下，選取&#x200B;**[!UICONTROL User Management]**。

   ![](assets/msi-actions-admin-guide-19.png)

1. 按一下&#x200B;**[!UICONTROL Actions]**&#x200B;並選取&#x200B;**[!UICONTROL Invite Users via CSV]**。

   ![](assets/msi-actions-admin-guide-20.png)

1. 瀏覽電腦上的CSV，選取並按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/msi-actions-admin-guide-21.png)

1. 確認欄位已正確對應，然後按一下&#x200B;**[!UICONTROL Invite]**。

   ![](assets/msi-actions-admin-guide-22.png)

邀請傳送後，您將會收到確認訊息。

>[!NOTE]
>
>完成此操作後，您可以升級現有的MSI封裝或安裝新的MSI封裝，然後繼續進行[在Salesforce中設定MSI動作](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}。
