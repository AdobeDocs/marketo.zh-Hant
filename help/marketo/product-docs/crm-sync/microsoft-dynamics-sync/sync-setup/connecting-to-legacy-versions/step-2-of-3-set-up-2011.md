---
unique-page-id: 3571807
description: 步驟3之2 — 在Dynamics中設定Marketo同步使用者（2011內部部署） - Marketo檔案 — 產品檔案
title: 步驟3之2 — 在Dynamics中設定Marketo同步使用者（2011內部部署）
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# 步驟3之2：在Dynamics中設定Marketo同步使用者（2011內部部署） {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

完成先前步驟的偉大工作，讓我們繼續探討這個問題。

>[!PREREQUISITES]
>
>[步驟3之1：安裝Marketo解決方案（2011年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)

## 指派同步使用者角色 {#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo外掛程式4.0.0.14版和更新版本。 對於舊版，所有使用者都必須擁有同步使用者角色。 若要升級Marketo，請參閱 [升級適用於Microsoft Dynamics的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步處理使用者的語言設定 [應該設定為英文](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 在左下角選單中，選取 **設定**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. 在樹狀結構中，選取 **管理**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. 選取 **使用者**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. 您將會在這裡看到使用者清單。 選取專屬的Marketo同步使用者，或連絡 [Active Directory同盟服務(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 管理員，以建立Marketo專屬的新使用者。 按一下 **管理角色**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. 檢查 **Marketo同步使用者** 並按一下 **確定**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >如果您沒有看到角色，請返回 [步驟3之1](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md) 並匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中所做的任何更新都將 **非** 已同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

即將完成！ 在前往下一篇文章之前，我們僅有最後幾項的設定。

1. 選取 **設定**. 然後選取 **Marketo設定** 在樹狀結構中。

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >如果缺少Marketo設定，請嘗試重新整理頁面。 如果問題持續存在， [再次發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md) 或登出再重新登入。

1. 按一下 **預設**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. 按一下 ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. 在快顯視窗中，選取同步使用者。 然後按一下 **確定**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. 按一下 **儲存** 以儲存變更。

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. 按一下 **發佈所有自訂**.

   ![](assets/publish-all-customizations1.png)

## 繼續進行步驟3之前 {#before-proceeding-to-step}

    *如果您想要限制同步處理的記錄數，請立即[設定自訂同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
    *執行[驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)程式。 它可驗證您的初始設定是否正確完成。
    *在Microsoft Dynamics CRM中登入Marketo Sync User。

做得好！

>[!MORELIKETHIS]
>
>[步驟3之3：將Microsoft Dynamics與Marketo連線（2011年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md)
