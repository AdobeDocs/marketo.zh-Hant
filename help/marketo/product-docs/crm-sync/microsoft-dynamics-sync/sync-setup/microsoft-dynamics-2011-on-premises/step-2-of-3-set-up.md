---
unique-page-id: 3571807
description: 第2步（共3步）-在Dynamics中設定Marketo同步用戶（2011年內部）-Marketo文檔——產品文檔
title: 第2步（共3步）-在Dynamics中設定Marketo同步用戶（2011年內部）
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# 步驟2（共3步）:在Dynamics（2011年內部部署）中設定Marketo同步用戶{#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

完成前述步驟的出色工作，讓我們繼續進行。

>[!PREREQUISITES]
>
>[步驟1（共3步）:安裝Marketo解決方案（2011年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## 分配同步用戶角色{#assign-sync-user-role}

將「Marketo同步用戶」角色僅分配給Marketo同步用戶。 您不需要將它指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo增效模組4.0.0.14版及更新版本。 對於舊版，所有使用者都必須具有同步使用者角色。 要升級Marketo，請參閱[升級MarketoMicrosoft Dynamics解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在左下角的菜單中，選擇&#x200B;**設定**。

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. 在樹中，選擇&#x200B;**管理**。

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. 選擇&#x200B;**用戶**。

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. 您會在這裡看到使用者清單。 選擇專用的Marketo同步用戶，或與[Active Directory聯合服務(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx)管理員聯繫，以建立專用於Marketo的新用戶。 按一下&#x200B;**管理角色**。

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. 選中&#x200B;**Marketo同步用戶** ，然後按一下&#x200B;**確定**。

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >如果您看不到角色，請返回至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)的[步驟1並匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新，都會將&#x200B;**not**&#x200B;同步回Marketo。

## 配置Marketo解決方案{#configure-marketo-solution}

快搞定了！ 在移至下一篇文章之前，我們只有最後幾段設定。

1. 選擇&#x200B;**設定**。 然後在樹中選擇&#x200B;**Marketo配置**。

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >如果缺少「Marketo配置」，請嘗試刷新頁面。 如果問題持續存在，[會再次發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)或登出並重新登入。

1. 按一下&#x200B;**Default**。

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. 按一下![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. 在彈出式選單中，選取同步使用者。 然後，按一下&#x200B;**確定**。

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. 按一下&#x200B;**保存**&#x200B;保存更改。

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. 按一下&#x200B;**發佈所有自定義**。

   ![](assets/publish-all-customizations1.png)

## 繼續執行步驟3 {#before-proceeding-to-step}之前

    *如果您想要限制同步的記錄數，請立即[設定自訂同步篩選](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
    *執行[驗證Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)程式。它會驗證您的初始設定是否正確完成。
    *在Microsoft Dynamics CRM中登入「Marketo同步使用者」。

幹得好！

>[!MORELIKETHIS]
>
>[步驟3（共3步）:將Microsoft Dynamics與Marketo（2011年內部部署）連接](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
