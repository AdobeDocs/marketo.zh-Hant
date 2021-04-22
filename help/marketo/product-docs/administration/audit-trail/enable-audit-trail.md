---
unique-page-id: 11382122
description: 啟用審計線索-Marketo文檔——產品文檔
title: 啟用審計線索
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# 啟用審核跟蹤{#enable-audit-trail}

稽核記錄可供所有客戶使用，並由兩個管理員權限控制。

>[!NOTE]
>
>依預設，所有系統管理員角色都啟用了這兩個權限。

## 啟用角色{#enable-audit-trail-for-a-role}的審計線索

1. 按一下&#x200B;**管理**。

   ![](assets/one-2.png)

1. 選擇&#x200B;**Users &amp; Roles** ，然後按一下&#x200B;**Roles**。

   ![](assets/two-2.png)

1. 選擇要啟用跟蹤線索的角色，然後按一下&#x200B;**編輯角色**。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >您也可以在此處選擇建立新角色並授予其「審核線索」訪問權限。

1. 展開&#x200B;**存取管理員**&#x200B;權限。 根據您的需求，選擇&#x200B;**存取稽核記錄**&#x200B;和／或&#x200B;**存取登入記錄**。 按一下&#x200B;**保存**。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**存取稽核記錄：** 讓使用者同時存取資產稽核記錄和管理稽核記錄。
   >
   >**存取登入記錄：** 讓使用者存取使 [用者登入記錄](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)。

## 為用戶{#assign-audit-trail-role-to-a-user}分配審計線索角色

>[!PREREQUISITES]
>
>[建](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) 立或啟 [](#enable-audit-trail) 用現有角色，賦予其「稽核記錄」權限。

1. 在&#x200B;**Users &amp; Roles**&#x200B;中，按一下&#x200B;**Users**。

   ![](assets/five-1.png)

1. 選擇要授予審計線索訪問權限的用戶，然後按一下&#x200B;**編輯用戶**。

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >當您建立新使用者時，也會套用此程式。

1. 選擇您建立的審計線索角色。 在此範例中，我們建立了「稽核記錄——資產和管理員」和「稽核記錄——包含登入記錄」。

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >如果已啟用工作區，請務必勾選角色的核取方塊，此核取方塊會選取所有工作區。 取消選取個別工作區將隱藏稽核記錄。 這表示您將會看到每個工作區的稽核記錄資料。 當[filtering](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)時，您可以選擇隱藏工作區。

1. 按一下&#x200B;**保存**。

   ![](assets/eight-1.png)
