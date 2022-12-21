---
unique-page-id: 11382122
description: 啟用稽核軌跡 — Marketo檔案 — 產品檔案
title: 啟用審核跟蹤
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
source-git-commit: 73d41904ca74ae265648c3ed91805be7c4d24fe0
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# 啟用審核跟蹤 {#enable-audit-trail}

稽核軌跡可供所有客戶使用，並由兩個管理權限控制。

>[!NOTE]
>
>依預設，所有系統管理員角色都已啟用這兩個權限。

## 啟用角色的稽核軌跡 {#enable-audit-trail-for-a-role}

1. 按一下 **管理**.

   ![](assets/enable-audit-trail-1.png)

1. 選擇 **使用者與角色** 按一下 **角色**.

   ![](assets/enable-audit-trail-2.png)

1. 選擇要為啟用審核跟蹤的角色，然後按一下 **編輯角色**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >您也可以選擇在此建立新角色，並授予其稽核軌跡存取權。

1. 展開 **存取管理員** 權限。 選擇 **存取稽核軌跡** 和/或 **訪問登錄歷史記錄**，視您的需求而定。 按一下 **儲存**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**訪問審核跟蹤：** 為使用者提供資產稽核軌跡和管理員稽核軌跡的存取權。
   >
   >**訪問登錄歷史記錄：** 提供使用者存取 [使用者登入歷史記錄](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## 將稽核軌跡角色指派給使用者 {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[建立](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) 或 [啟用](#enable-audit-trail) 現有角色，授予其稽核軌跡權限。

1. 在 **使用者與角色**，按一下 **使用者**.

   ![](assets/enable-audit-trail-5.png)

1. 選取您要授予稽核軌跡存取權的使用者，然後按一下 **編輯用戶**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >建立新使用者時，也適用此程式。

1. 選擇您建立的審核跟蹤角色。 在此範例中，我們建立了「稽核軌跡 — 資產和管理員」和「稽核軌跡 — 包含登入歷史記錄」。

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >如果已啟用工作區，請務必勾選角色的核取方塊，以選取所有工作區。 取消選取個別工作區會隱藏稽核軌跡。 這表示您會看到每個工作區的稽核軌跡資料。 您確實可以選擇在 [篩選](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. 按一下 **儲存**.

   ![](assets/enable-audit-trail-8.png)
