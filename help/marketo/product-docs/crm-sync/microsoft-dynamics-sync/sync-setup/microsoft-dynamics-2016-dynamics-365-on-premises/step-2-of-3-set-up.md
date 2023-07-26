---
description: 安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟2之3 - Marketo檔案 — 產品檔案
title: 安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟2之3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 步驟3之2：設定Marketo for Dynamics （2016內部部署/Dynamics 365內部部署）{#step-of-set-up-for-marketo-on-premises-2016}

完成上述步驟的絕佳工作。 讓我們繼續討論這個問題。

>[!PREREQUISITES]
>
>[安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟3之1](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## 建立新使用者 {#create-a-new-user}

1. 登入Dynamics。 按一下「設定」圖示並選取「進階設定」。

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. 按一下 **設定** 並選取 **安全性**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. 按一下 **使用者**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. 按一下 **新增**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. 按一下 **新增並授權使用者**. 新標籤應會開啟。

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. 按一下 **管理員** ，位於頁面頂端。 另一個新標籤應會開啟。

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. 按一下 **新增使用者**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. 輸入您的所有資訊。 完成後，按一下 **新增**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >此名稱必須是專用的同步處理使用者，而非現有的CRM使用者帳戶。 它不需要是實際的電子郵件地址。

1. 輸入要接收新使用者認證的電子郵件，然後按一下「傳送電子郵件並關閉」。

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## 建立新的使用者端應用程式 {#create-a-new-client-application}

請依照中的步驟操作 [此Microsoft文章](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) 建立新的使用者端應用程式並授與許可權。 請記下Dynamics使用者端應用程式的使用者端ID/密碼。

## 指派同步使用者角色 {#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo 4.0.0.14版和更新版本。 對於舊版，所有使用者都必須擁有同步使用者角色。 若要升級Marketo，請參閱 [升級適用於Microsoft Dynamics的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步處理使用者的語言設定 [應該設定為英文](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 在 **設定**，按一下 **安全性**.

   ![](assets/assign1.png)

1. 按一下 **使用者**.

   ![](assets/assign2.png)

1. 您將會在這裡看到使用者清單。 選取專屬的Marketo Sync使用者，或聯絡 [Active Directory同盟服務](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理員，為Marketo建立專屬使用者。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選取同步使用者。 按一下 **管理角色**.

   ![](assets/assign4.png)

   勾選「Marketo同步處理使用者」 ，然後按一下「確定」。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果您沒有看到角色，請返回 [步驟3之1](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) 並匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中所做的任何更新都將 **非** 已同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

即將完成！ 在前往下一篇文章之前，我們僅有最後幾項的設定。

1. 在 **設定**，按一下 **Marketo設定**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo設定，請嘗試重新整理頁面。 如果問題持續存在， [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) 或嘗試登出再重新登入。

1. 按一下 **預設**.

   ![](assets/configure2.png)

1. 按一下 **Marketo使用者** 欄位並選取同步使用者。

   ![](assets/configure3.png)

1. 按一下右下角的儲存圖示。

   ![](assets/configure4.png)

1. 按一下 **發佈所有自訂**.

   ![](assets/publish-all-customizations1.png)

## 繼續進行步驟3之前 {#before-proceeding-to-step}

* 如果要限制同步處理的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 立即。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 程式。 它可驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入Marketo Sync User。

>[!MORELIKETHIS]
>
>[安裝Marketo for Microsoft Dynamics 2016/Dynamics 365內部部署步驟3之3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
