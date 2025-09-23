---
unique-page-id: 2359909
description: 管理使用者角色和許可權 — Marketo檔案 — 產品檔案
title: 管理使用者角色和權限
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
feature: Users and Roles
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 7%

---

# 管理使用者角色和權限 {#managing-user-roles-and-permissions}

設定、建立和編輯使用者角色，並將它們指派給使用者。 這可讓您控制每個Marketo使用者有權存取的區域與功能。

例如，行銷使用者通常需要跨應用程式的廣泛存取權，才能建立、修改和部署電子郵件、登入頁面和方案。 另一方面，網頁設計人員幾乎將所有時間都花在Design Studio中，建立資產以用於電子郵件和登陸頁面。 雖然公司領導在Analytics區域中廣泛使用Marketo的報告，但可能不需要自行建立或推動資產或計畫。

>[!NOTE]
>
>**需要管理員許可權**

Marketo提供數個內建角色，具有不同的存取層級：

* **管理員** — 應用程式的所有部分，包括管理員區段
* **標準使用者** — 應用程式的所有部分，管理區段除外
* **行銷使用者** — 應用程式的所有部分，管理區段除外
* **網頁Designer** — 僅限設計工作室
* **Analytics使用者** — 僅限Analytics區段

您無法編輯「管理員」和「標準使用者」角色，但可以編輯其他角色。 您也可以建立新的自訂角色，以符合公司中的特定組織結構。

## Marketo 與 Adobe Identity {#marketo-with-adobe-identity}

如果您使用Marketo搭配Adobe Identity，您可以在此找到[設定檔說明清單](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels)。

## 將角色指派給使用者 {#assign-roles-to-a-user}

當您[第一次建立使用者](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md)或[編輯現有的使用者](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)時，您可以將角色指派給使用者。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/managing-user-roles-and-permissions-1.png)

1. 按一下「**[!UICONTROL Users & Roles]**」。

   ![](assets/managing-user-roles-and-permissions-2.png)

1. 從清單中選取您要編輯的使用者，然後按一下&#x200B;**[!UICONTROL Edit User]**。

   ![](assets/managing-user-roles-and-permissions-3.png)

1. 在「**[!UICONTROL Roles]**」下，根據使用者需要的許可權，選取您要指派給使用者的角色，然後按一下「**[!UICONTROL Save]**」。

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >若要瞭解每個角色，請參閱[角色許可權說明](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md)。

## 建立新角色 {#create-a-new-role}

有時候，您的組織會有具有非常特定角色的員工，這些角色需要自訂許可權組合。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/managing-user-roles-and-permissions-5.png)

1. 按一下「**[!UICONTROL Users & Roles]**」。

   ![](assets/managing-user-roles-and-permissions-6.png)

1. 按一下「**[!UICONTROL Roles]**」標籤。

   ![](assets/managing-user-roles-and-permissions-7.png)

1. 按一下「**[!UICONTROL New Role]**」。

   ![](assets/managing-user-roles-and-permissions-8.png)

1. 輸入&#x200B;**[!UICONTROL Role Name]**、**[!UICONTROL Description]** （選擇性），然後選取此角色中的使用者需要的許可權。

   ![](assets/managing-user-roles-and-permissions-9.png)

## 編輯角色 {#edit-a-role}

如果您需要變更與現有角色相關聯的許可權，可以編輯角色。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/managing-user-roles-and-permissions-10.png)

1. 按一下「**[!UICONTROL Users & Roles]**」。

   ![](assets/managing-user-roles-and-permissions-11.png)

1. 按一下「**[!UICONTROL Roles]**」標籤。

   ![](assets/managing-user-roles-and-permissions-12.png)

1. 從清單中選取您要修改的角色，然後按一下&#x200B;**[!UICONTROL Edit Role]**。

   ![](assets/managing-user-roles-and-permissions-13.png)

1. 必要時變更&#x200B;**[!UICONTROL Role Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**、變更相關&#x200B;**[!UICONTROL Permissions]**&#x200B;的選取專案，並在完成時按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >擁有您編輯之角色的使用者在登出後再重新登入後，將會收到修改過的許可權。

## 刪除角色 {#delete-a-role}

如果某個角色變得不必要，您可以將其刪除。

1. 前往「**[!UICONTROL Admin]**」區域。

   ![](assets/managing-user-roles-and-permissions-15.png)

1. 按一下「**[!UICONTROL Users & Roles]**」。

   ![](assets/managing-user-roles-and-permissions-16.png)

1. 按一下「**[!UICONTROL Roles]**」標籤。

   ![](assets/managing-user-roles-and-permissions-17.png)

1. 從清單中選取您要刪除的角色，然後按一下&#x200B;**[!UICONTROL Delete Role]**。

   ![](assets/managing-user-roles-and-permissions-18.png)

1. 按一下&#x200B;**[!UICONTROL Delete]**&#x200B;確認。

   ![](assets/managing-user-roles-and-permissions-19.png)
