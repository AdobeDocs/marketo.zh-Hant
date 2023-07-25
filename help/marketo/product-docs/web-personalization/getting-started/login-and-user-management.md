---
unique-page-id: 7513771
description: 登入和使用者管理 — Marketo檔案 — 產品檔案
title: 登入和使用者管理
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 登入和使用者管理 {#login-and-user-management}

## 建立Web個人化使用者角色 {#create-a-web-personalization-user-role}

1. 前往 **管理員** 區段，然後按一下 **使用者和角色**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. 按一下 **角色**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >如果Web Personalization (WP)使用者角色已存在，請確定已將其設定為如步驟4中所示。

1. 按一下 **新角色**.

   ![](assets/three-1.png)

1. 輸入角色名稱並選取許可權。 按一下 **建立** (此角色必須 [套用至所有工作區](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md))。

   ![](assets/four.png)

   >[!TIP]
   >
   >若要授予使用者存取「鎖定目標」和「個人化」中所有專案的許可權，請務必選取 _全部_ 核取方塊。

## Web個人化和預測性內容使用者許可權 {#web-personalization-and-predictive-content-user-permissions}

**目標定位和個人化**：使用者只有檢視許可權（若僅選取此許可權）。

**管理網頁個人化+預測性**：使用者只能存取網頁個人化和預測性內容應用程式的「帳戶設定」和「內容設定」。 使用者可以檢視應用程式中的頁面，但沒有建立、編輯、刪除和啟動許可權。

**預測性內容編輯器**：使用者擁有預測內容應用程式的編輯器存取權。 此許可權可讓您建立、編輯、刪除內容片段。 不允許在網頁或電子郵件上啟用預測性使用內容。

**預測性內容啟動器**：使用者可存取所有預測性內容功能，但「帳戶」和「內容設定」除外。 此許可權可讓您建立、編輯和刪除及啟用內容片段。

**網站行銷活動編輯器**：使用者擁有所有Web個人化功能的編輯器存取權，可建立、編輯和刪除但不啟動Web行銷活動。

**Web Campaign啟動器**：使用者可存取所有Web個人化應用程式功能，但「帳戶」和「內容設定」除外。 此許可權可讓您建立、編輯、刪除和啟動網站行銷活動。

## 將WP角色指派給使用者 {#assign-wp-role-to-user}

1. 前往 **使用者**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. 選取要授予WP存取權的使用者，然後按一下 **編輯使用者**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. 選取所有工作區的WP使用者角色。

   ![](assets/seven.png)

1. 新啟用的使用者將會看到 **網頁個人化** 圖磚(在「我的Marketo」中顯示)。

   ![](assets/eight.png)
