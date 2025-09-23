---
unique-page-id: 11382122
description: 啟用稽核軌跡 — Marketo檔案 — 產品檔案
title: 啟用稽核軌跡
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 5%

---

# 啟用稽核軌跡 {#enable-audit-trail}

稽核軌跡可供所有客戶使用，並受兩個管理員許可權控制。

>[!NOTE]
>
>依預設，所有系統管理員角色都會啟用這兩個許可權。

## 啟用角色的稽核軌跡 {#enable-audit-trail-for-a-role}

1. 按一下「**[!UICONTROL Admin]**」。

   ![](assets/enable-audit-trail-1.png)

1. 選取「**[!UICONTROL Users & Roles]**」然後按一下「**[!UICONTROL Roles]**」。

   ![](assets/enable-audit-trail-2.png)

1. 選取您要啟用稽核軌跡的角色，然後按一下&#x200B;**[!UICONTROL Edit Role]**。

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >您也可以在這裡選擇建立新角色，並授予其稽核軌跡存取權。

1. 展開&#x200B;**[!UICONTROL Access Admin]**&#x200B;許可權。 根據您的需求，選取&#x200B;**[!UICONTROL Access Audit Trail]**&#x200B;及/或&#x200B;**[!UICONTROL Access Login History]**。 按一下「**[!UICONTROL Save]**」。

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**[!UICONTROL Access Audit Trail]**：授與使用者存取[!UICONTROL Asset Audit Trail]和[!UICONTROL Admin Audit Trail]的許可權。
   >
   >**[!UICONTROL Access Login History]**：授予使用者[使用者登入歷程記錄](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)的存取權。

## 指派稽核軌跡角色給使用者 {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[建立](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role)或[啟用](#enable-audit-trail)現有的角色，賦予其稽核軌跡許可權。

1. 在&#x200B;**[!UICONTROL Users & Roles]**&#x200B;中，按一下&#x200B;**[!UICONTROL Users]**。

   ![](assets/enable-audit-trail-5.png)

1. 選取您要授與稽核軌跡存取權的使用者，然後按一下&#x200B;**[!UICONTROL Edit User]**。

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >建立新使用者時，此程式也適用。

1. 選取您建立的稽核軌跡角色。 在此範例中，我們建立了「稽核軌跡 — 資產和管理員」以及「稽核軌跡 — 包含登入歷史記錄」。

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >如果您已啟用工作區，請務必勾選角色的核取方塊，以選取所有工作區。 取消選取個別工作區將會隱藏稽核軌跡。 這表示您會看到每個工作區的稽核軌跡資料。 當[篩選](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)時，您可以選擇隱藏工作區。

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/enable-audit-trail-8.png)
