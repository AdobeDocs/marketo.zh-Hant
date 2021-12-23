---
unique-page-id: 3571816
description: 第2步（共3步） — 為Marketo配置同步用戶（2013年內部部署） — Marketo文檔 — 產品文檔
title: 第2步（共3步） — 為Marketo配置同步用戶（2013年內部部署）
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 第2步（共3步）:為Marketo配置同步用戶（2013年內部部署） {#step-of-configure-sync-user-for-marketo-on-premises}

完成上述步驟非常好，讓我們繼續完成。

>[!PREREQUISITES]
>
>[第1步（共3步）:在Dynamics（2013內部部署）中安裝Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## 分配同步用戶角色 {#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo外掛程式4.0.0.14版和更新版本。 對於較舊版本，所有使用者都必須具有同步使用者角色。 若要升級Marketo，請參閱 [升級Microsoft Dynamics的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步用戶的語言設定 [應設為英文](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 在 **設定**，按一下 **管理**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 選擇 **使用者**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您會在此處看到使用者清單。 選取您專屬的Marketo Sync使用者，或聯絡您的 [Active Directory聯合身份驗證服務(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理員，以建立專屬於Marketo的新使用者。](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 按一下 ![](assets/image2015-3-26-11-3a16-3a22.png) 選取 **管理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 檢查 **Marketo同步使用者** 按一下 **確定**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >如果您沒有看見角色，請返回 [步驟1至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) 並匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新都將 **not** 同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

快完成了！ 我們只有最後幾段配置，然後再轉到下一篇文章。

1. 在 **設定**，按一下 **Marketo設定**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >若 **Marketo設定** 遺失，請嘗試重新整理頁面。 如果問題持續存在， [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) 請再次登出，或嘗試重新登入。

1. 按一下 **預設**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 按一下 **Marketo使用者** 欄位，然後選取同步使用者。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 按一下 ![](assets/image2015-3-13-15-3a10-3a11.png) 的下方以儲存變更。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 按一下 **發佈所有自訂**.

   ![](assets/publish-all-customizations1.png)

## 繼續執行步驟3之前 {#before-proceeding-to-step}

* 如果要限制同步的記錄數， [設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 現在。
* 執行 [驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 程式。 它會驗證您的初始設定是否正確執行。
* 在Microsoft Dynamics CRM中登入Marketo同步使用者。

幹得好！

>[!MORELIKETHIS]
>
>[第3步（共3步）:連接Marketo和Dynamics（2013年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
