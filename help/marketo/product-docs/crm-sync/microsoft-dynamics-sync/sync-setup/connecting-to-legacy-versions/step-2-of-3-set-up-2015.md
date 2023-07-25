---
unique-page-id: 7504739
description: 安裝Marketo for Microsoft Dynamics 2015內部部署步驟2之3 - Marketo檔案 — 產品檔案
title: 安裝Marketo for Microsoft Dynamics 2015內部部署步驟2/3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 步驟3之2：設定Marketo for Dynamics （2015內部部署）{#step-of-set-up-for-marketo-on-premises-2015}

完成上述步驟的絕佳工作。 讓我們繼續討論這個問題。

>[!PREREQUISITES]
>
>[安裝Marketo for Microsoft Dynamics 2015內部部署步驟1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)

## 指派同步使用者角色 {#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo 4.0.0.14版和更新版本。 對於舊版，所有使用者都必須擁有同步使用者角色。 若要升級Marketo，請參閱 [升級適用於Microsoft Dynamics的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步處理使用者的語言設定 [應該設定為英文](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 下 **設定**，按一下 **安全性**.

   ![](assets/assign1.png)

1. 按一下 **使用者**.

   ![](assets/assign2.png)

1. 您將會在這裡看到使用者清單。 選取專屬的Marketo Sync使用者，或聯絡 [Active Directory同盟服務](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理員，為Marketo建立專屬使用者。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選取同步使用者。 按一下 **管理角色**.

   ![](assets/assign4.png)

1. 檢查Marketo同步使用者並按一下 **確定**.

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >同步處理使用者應該要有Marketo設定的讀取許可權。

   >[!TIP]
   >
   >如果您沒有看到角色，請返回 [步驟1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) 並匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中所做的任何更新都將 **not** 已同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

即將完成！ 在前往下一篇文章之前，我們僅剩下幾項設定。

1. 下 **設定**，按一下 **Marketo設定**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo Config，請嘗試重新整理頁面。 如果問題持續存在， [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) 或嘗試登出再重新登入。

1. 按一下 **預設**.

   ![](assets/configure2.png)

1. 按一下 **Marketo使用者** 欄位並選取同步使用者。

   ![](assets/configure3.png)

1. 按一下右下角的儲存圖示。

   ![](assets/configure4.png)

1. 按一下 **發佈所有自訂**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >同步處理使用者應該要有Marketo設定的讀取許可權。

## 繼續進行步驟3之前 {#before-proceeding-to-step}

* 如果要限制同步處理的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 立即。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 程式。 它可驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入Marketo Sync使用者。

>[!MORELIKETHIS]
>
>[安裝Marketo for Microsoft Dynamics 2015內部部署步驟3之3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md)
