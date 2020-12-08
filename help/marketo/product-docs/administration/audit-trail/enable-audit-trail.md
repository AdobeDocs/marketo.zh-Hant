---
unique-page-id: 11382122
description: 啟用稽核記錄——行銷人員檔案——產品檔案
title: 啟用審計線索
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 啟用審計線索 {#enable-audit-trail}

稽核記錄可供所有客戶使用，並由兩個管理員權限控制。

>[!NOTE]
>
>依預設，所有系統管理員角色都啟用了這兩個權限。

## 為角色啟用審計線索 {#enable-audit-trail-for-a-role}

1. 按一 **下管理**。

   ![](assets/one-2.png)

1. 選擇「 **用戶和角色** 」，然後按一下「 **角色」**。

   ![](assets/two-2.png)

1. 選擇要啟用跟蹤線索的角色，然後按一下編 **輯角色**。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >您也可以在此處選擇建立新角色並授予其「審核線索」訪問權限。

1. 展開「存 **取管理員** 」權限。 根據 **您的需求，選擇「存取稽核記錄** 」和/ **或「存取登入記錄**」。 按一下 **儲存**。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**定義**
   >
   >
   >**存取稽核記錄：** 為使用者提供資產稽核記錄和管理稽核記錄的存取權。
   >
   >
   >**存取登入記錄：** 為使用者提供使用者登 [入記錄的存取權](user-login-history.md)。

## 將審核跟蹤角色分配給用戶 {#assign-audit-trail-role-to-a-user}

>[!NOTE]
>
>**必要條件**
>
>[建立](http://docs.marketo.com/display/DOCS/Create,+Delete,+Edit+and+Change+a+User+Role#Create,Delete,EditandChangeaUserRole-CreateaRole) 或 [啟用](#Enable) 現有角色，賦予其「稽核記錄」權限。

1. 在「使 **用者與角色**」中，按一 **下「使用者」**。

   ![](assets/five-1.png)

1. 選擇要授予審計線索訪問權限的用戶，然後按一下編輯 **用戶**。

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >當您建立新使用者時，也會套用此程式。

1. 選擇您建立的審計線索角色。 在此範例中，我們建立了「稽核記錄——資產和管理員」和「稽核記錄——包含登入記錄」。

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >如果已啟用工作區，請務必勾選角色的核取方塊，此核取方塊會選取所有工作區。 取消選取個別工作區將隱藏稽核記錄。 這表示您將會看到每個工作區的稽核記錄資料。 您確實可以在篩選時隱藏工作 [區](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)。

1. 按一下 **儲存**。

   ![](assets/eight-1.png)

