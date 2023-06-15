---
description: Sales Insight Actions管理員設定指南 — Marketo檔案 — 產品檔案
title: Sales Insight Actions管理員設定指南
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Sales Insight Actions管理員設定指南 {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions是以Web為基礎的應用程式，可透過 [Marketo Sales Insight套件](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. 有時稱為「Marketo銷售」，或簡稱為「動作」。

>[!PREREQUISITES]
>
>* 向Adobe帳戶團隊（您的帳戶管理員）確認已為您的Marketo Engage帳戶啟用MSI動作(如果您沒有帳戶管理員，請聯絡 [Marketo支援](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"})。
>* 必須設定您的Marketo/Salesforce同步處理。

<table>
 <tr>
  <th>角色</th>
  <th>步驟</th>
 </tr>
 <tr>
  <td>Marketo管理員</td>
  <td>設定Marketo銷售帳戶</td>
 </tr>
 <tr>
  <td>Marketo管理員或 <br/>Salesforce管理員</td>
  <td>將Marketo Sales帳戶連結至Salesforce</td>
 </tr>
 <tr>
  <td>Marketo管理員</td>
  <td>將Marketo銷售帳戶連線至Marketo</td>
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
  <td>Salesforce管理員</td>
  <td>在Salesforce中安裝/升級MSI套件</td>
 </tr>
 <tr>
  <td>Salesforce管理員</td>
  <td>在Salesforce中設定MSI-Actions</td>
 </tr>
</table>

## 設定Marketo銷售帳戶 {#set-up-marketo-sales-account}

1. 在Marketo中，按一下 **管理員**.

   ![](assets/msi-actions-admin-guide-1.png)

1. 按一下 **銷售分析**，則 **動作設定**. 從Marketo管理員清單中選取以邀請並點選 **傳送邀請**.

   ![](assets/msi-actions-admin-guide-2.png)

使用者會收到電子郵件，其中包含存取帳戶的步驟。

>[!NOTE]
>
>其他使用者不會透過Marketo新增，而是透過「銷售帳戶使用者管理」頁面新增。 [按一下這裡](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"} 以進一步瞭解如何新增其他使用者。

## 將Marketo銷售帳戶連結至Salesforce {#connect-marketo-sales-account-to-salesforce}

1. 在您的Marketo Sales帳戶中，按一下齒輪圖示並選取 **設定**.

   ![](assets/msi-actions-admin-guide-3.png)

1. 在「管理設定」底下，按一下 **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. 在「連線和自訂」標籤中，按一下 **Connect**.

   ![](assets/msi-actions-admin-guide-5.png)

1. 按一下 **確定**.

   ![](assets/msi-actions-admin-guide-6.png)

如果您已登入Salesforce，則會與您連線。 否則系統會要求您登入。

## 將Marketo連線至您的Sales Apps帳戶 {#connect-marketo-to-your-sales-apps-account}

1. 在您的Marketo Sales帳戶中，按一下齒輪圖示並選取 **設定**.

   ![](assets/msi-actions-admin-guide-7.png)

1. 在「管理設定」底下，按一下 **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. 按一下 **connect**. 然後會連線您的帳戶。

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>如果未連線，請從Marketo Sales Insight的「動作設定」索引標籤複製認證，然後貼到「設定」索引標籤中。

## 啟動資料同步 {#initiate-data-sync}

Sales Insight Actions的資料統一欄位同步可讓系統從Marketo Engage資料庫將人員資訊提取到Sales Insight Actions資料庫中，讓您的人員資料保持最新，並確保活動記錄到Marketo和Salesforce的正確記錄中。

>[!CAUTION]
>
>啟動資料同步處理後，您應該 **not** 移除銷售分析動作例項上的原始使用者。 這是第一個邀請收件者的使用者。

1. 在Marketo中，按一下 **管理員**.

   ![](assets/msi-actions-admin-guide-10.png)

1. 按一下 **銷售分析**.

   ![](assets/msi-actions-admin-guide-11.png)

1. 按一下 **動作設定** 標籤。 在動作欄位同步卡中，按一下 **同步**.

   ![](assets/msi-actions-admin-guide-12.png)

1. 您將看到將同步的欄位預覽。 按一下 **開始同步**.

   ![](assets/msi-actions-admin-guide-13.png)

Marketo和Salesforce中存在的個人記錄將同步至您的Marketo Sales Apps帳戶。

>[!NOTE]
>
>若要進一步瞭解人員與活動資料如何在Sales Insight Actions、Marketo和Salesforce之間同步， [按一下這裡](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}.

## 邀請個別使用者加入MSI動作 {#invite-individual-users-to-msi-actions}

1. 在您的Marketo Sales帳戶中，按一下齒輪圖示並選取 **設定**.

   ![](assets/msi-actions-admin-guide-14.png)

1. 在「管理設定」下，選取 **User Management**.

   ![](assets/msi-actions-admin-guide-15.png)

1. 按一下 **動作** 並選取 **邀請使用者**.

   ![](assets/msi-actions-admin-guide-16.png)

1. 輸入電子郵件地址並按一下 **邀請**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>依預設，所有新成員都會新增至「所有人」團隊。

您將會收到確認訊息。

## 透過CSV邀請使用者加入MSI動作 {#invite-users-via-csv-to-msi-actions}

1. 在您的Marketo Sales帳戶中，按一下齒輪圖示並選取 **設定**.

   ![](assets/msi-actions-admin-guide-18.png)

1. 在「管理設定」下，選取 **User Management**.

   ![](assets/msi-actions-admin-guide-19.png)

1. 按一下 **動作** 並選取 **透過CSV邀請使用者**.

   ![](assets/msi-actions-admin-guide-20.png)

1. 在電腦上瀏覽CSV，選取並按一下 **下一個**.

   ![](assets/msi-actions-admin-guide-21.png)

1. 確認欄位已正確對應，然後按一下 **邀請**.

   ![](assets/msi-actions-admin-guide-22.png)

邀請傳送後，您將會收到確認訊息。

>[!NOTE]
>
>完成此操作後，您可以升級現有的MSI套件或安裝新的MSI套件並移至 [在Salesforce中設定MSI動作](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}.
