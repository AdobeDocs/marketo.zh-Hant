---
unique-page-id: 7504739
description: Install Marketo for Microsoft Dynamics 2015 On-Premises Step 2 of 3 - Marketo Docs - Product Documentation
title: 安裝Marketo for Microsoft Dynamics 2015內部部署步驟2（共3個）
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 7b1f0d0d45bbfe3d8b781282e0a4ef1884a2bf40
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 設定Dynamics Marketo的步驟2（2015年上線）{#step-of-set-up-for-marketo-on-premises-2015}

Great job completing the previous steps. 讓我們繼續過去。

>[!PREREQUISITES]
>
>[Install Marketo for Microsoft Dynamics 2015 On-Premises Step 1 of 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)

## 分配同步用戶角色 {#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
>
>This applies to Marketo version 4.0.0.14 and later. 對於較舊版本，所有使用者都必須具有同步使用者角色。 若要升級您的Marketo，請參閱 [升級Microsoft Dynamics的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步用戶的語言設定 [應設為英文](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Under **Settings**, click **Security**.

   ![](assets/assign1.png)

1. Click **Users**.

   ![](assets/assign2.png)

1. 您會在此處看到使用者清單。 Select the dedicated Marketo Sync user or contact your [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) administrator to create a dedicated user for Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 Click **Manage Roles**.

   ![](assets/assign4.png)

   Check Marketo Sync User and click OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果您沒有看見角色，請返回 [步驟1至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) 並匯入解決方案。

   >[!NOTE]
   >
   >Any updates made in your CRM by the Sync User will **not** be synced back to Marketo.

## 設定Marketo解決方案 {#configure-marketo-solution}

快完成了！ We just have a few last pieces of configuration before moving onto the next article.

1. Under **Settings**, click **Marketo Config**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo設定，請嘗試重新整理頁面。 If the issue persists, [publish the Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) or try logging out and back in.

1. 按一下 **預設**.

   ![](assets/configure2.png)

1. Click the **Marketo User** field and select the sync user.

   ![](assets/configure3.png)

1. 按一下右下角的儲存圖示。

   ![](assets/configure4.png)

1. 按一下 **發佈所有自訂**.

   ![](assets/publish-all-customizations1.png)

## 繼續執行步驟3之前 {#before-proceeding-to-step}

* 如果要限制同步的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 現在。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 程式。 它會驗證您的初始設定是否正確執行。
* 登入Microsoft Dynamics CRM中的Marketo同步使用者。

>[!MORELIKETHIS]
>
>[安裝Marketo for Microsoft Dynamics 2015內部部署步驟3（共3個）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md)
