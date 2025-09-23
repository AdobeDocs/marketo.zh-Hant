---
unique-page-id: 7513771
description: 登入與使用者管理 — Marketo檔案 — 產品檔案
title: 登入及使用者管理
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 3%

---

# 登入及使用者管理 {#login-and-user-management}

## 建立[!UICONTROL Web Personalization]使用者角色 {#create-a-web-personalization-user-role}

1. 移至&#x200B;**[!UICONTROL Admin]**&#x200B;區段，然後按一下&#x200B;**[!UICONTROL Users & Roles]**。

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. 按一下「**[!UICONTROL Roles]**」。

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >如果網頁Personalization (WP)使用者角色已經存在，請確定它已依照步驟4進行設定。

1. 按一下「**[!UICONTROL New Role]**」。

   ![](assets/three-1.png)

1. 輸入[!UICONTROL Role Name]並選取[!UICONTROL Permissions]。 按一下&#x200B;**[!UICONTROL Create]** （此角色必須[套用至所有工作區](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)）。

   ![](assets/four.png)

   >[!TIP]
   >
   >若要授予使用者存取定位和Personalization中所有專案的許可權，請務必選取&#x200B;_所有_&#x200B;核取方塊。

## [!UICONTROL Web Personalization]和預測性內容使用者許可權 {#web-personalization-and-predictive-content-user-permissions}

**[!UICONTROL Targeting and Personalization]**：如果只選取此許可權，則使用者具有僅檢視許可權。

**[!UICONTROL Admin Web Personalization + Predictive]**：使用者只能存取網頁Personalization和預測性內容應用程式的「帳戶設定」和「內容設定」。 使用者可以在應用程式中檢視頁面，但沒有建立、編輯、刪除、啟動許可權。

**[!UICONTROL Predictive Content Editor]**：使用者擁有預測內容應用程式的編輯器存取權。 此許可權可讓您建立、編輯、刪除內容片段。 不允許在網頁或電子郵件上啟用預測用途的內容。

**[!UICONTROL Predictive Content Launcher]**：使用者可存取所有預測性內容功能，但[帳戶]和[內容設定]除外。 此許可權可讓您建立、編輯和刪除及啟用內容片段。

**[!UICONTROL Web Campaign Editor]**：使用者擁有所有Web Personalization功能的編輯器存取權，可以建立、編輯和刪除但不啟動Web行銷活動。

**[!UICONTROL Web Campaign Launcher]**：使用者可存取所有Web Personalization應用程式功能，但[帳戶]和[內容設定]除外。 此許可權可讓您建立、編輯、刪除和啟動網頁行銷活動。

## 指派WP角色給使用者 {#assign-wp-role-to-user}

1. 移至&#x200B;**[!UICONTROL Users]**。

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. 選取要授予WP存取許可權的使用者，然後按一下&#x200B;**[!UICONTROL Edit User]**。

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. 選取所有工作區的WP使用者角色。

   ![](assets/seven.png)

1. 新啟用的使用者下次登入時，將會在「我的Marketo」中看到&#x200B;**[!UICONTROL Web Personalization]**&#x200B;圖磚。

   ![](assets/eight.png)
