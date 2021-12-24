---
description: Install Marketo for Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 2 of 3 - Marketo Docs - Product Documentation
title: 安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟2（共3步）
source-git-commit: 7b1f0d0d45bbfe3d8b781282e0a4ef1884a2bf40
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 設定Dynamics Marketo的第2步（2016年內部部署/Dynamics 365內部部署）{#step-of-set-up-for-marketo-on-premises-2016}

完成前述步驟非常好。 讓我們繼續過去。

>[!PREREQUISITES]
>
>[安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟1（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## 分配同步用戶角色 {#assign-sync-user-role}

Assign the Marketo Sync User role only to the Marketo sync user. 您不需要將其指派給任何其他使用者。

>[!NOTE]
>
>This applies to Marketo version 4.0.0.14 and later. 對於較舊版本，所有使用者都必須具有同步使用者角色。 To upgrade your Marketo, see [Upgrade the Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步用戶的語言設定 [應設為英文](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 在 **設定**，按一下 **安全性**.

   ![](assets/assign1.png)

1. 按一下 **使用者**.

   ![](assets/assign2.png)

1. You will see a list of users here. 選取專屬的Marketo Sync使用者，或聯絡您的 [Active Directory聯合身份驗證服務](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理員，為Marketo建立專用使用者。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 Click **Manage Roles**.

   ![](assets/assign4.png)

   檢查Marketo同步用戶，然後按一下確定。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果您沒有看見角色，請返回 [步驟1至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) 並匯入解決方案。

   >[!NOTE]
   >
   >Any updates made in your CRM by the Sync User will **not** be synced back to Marketo.

## 設定Marketo解決方案 {#configure-marketo-solution}

Almost done! We just have a few last pieces of configuration before moving onto the next article.

1. Under **Settings**, click **Marketo Config**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >If Marketo Config is missing, try refreshing the page. 如果問題持續存在， [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) 或嘗試登出再登入。

1. Click **Default**.

   ![](assets/configure2.png)

1. Click the **Marketo User** field and select the sync user.

   ![](assets/configure3.png)

1. 按一下右下角的儲存圖示。

   ![](assets/configure4.png)

1. 按一下 **發佈所有自訂**.

   ![](assets/publish-all-customizations1.png)

## Before Proceeding to Step 3 {#before-proceeding-to-step}

* If you want to restrict the number of records you sync, [set up a custom sync filter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) now.
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 程式。 It verifies that your initial setups were done correctly.
* Log in to the Marketo Sync User in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟3（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
