---
unique-page-id: 3571816
description: 步驟2（共3步）-為Marketo（2013年內部部署）配置同步用戶-Marketo文檔——產品文檔
title: 步驟2（共3步）-為Marketo（2013年內部）配置同步用戶
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 步驟2（共3步）:為Marketo配置同步用戶（2013內部）{#step-of-configure-sync-user-for-marketo-on-premises}

完成前述步驟的出色工作，讓我們繼續進行。

>[!PREREQUISITES]
>
>[步驟1（共3步）:在Dynamics中安裝Marketo解決方案（2013年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## 分配同步用戶角色{#assign-sync-user-role}

將「Marketo同步用戶」角色僅分配給Marketo同步用戶。 您不需要將它指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo增效模組4.0.0.14版及更新版本。 對於舊版，所有使用者都必須具有同步使用者角色。 要升級Marketo，請參閱[升級MarketoMicrosoft Dynamics解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在&#x200B;**Settings**&#x200B;下，按一下&#x200B;**Administration**。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 選擇&#x200B;**用戶**。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您會在這裡看到使用者清單。 選擇專用的Marketo同步用戶或聯繫您的[Active Directory聯合服務(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理員以建立專用於Marketo的新用戶。](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 按一下![](assets/image2015-3-26-11-3a16-3a22.png)並選擇&#x200B;**管理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 選中&#x200B;**Marketo同步用戶** ，然後按一下&#x200B;**確定**。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >如果您看不到角色，請返回至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)的[步驟1並匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新，都會將&#x200B;**not**&#x200B;同步回Marketo。

## 配置Marketo解決方案{#configure-marketo-solution}

快搞定了！ 在移至下一篇文章之前，我們只有最後幾段設定。

1. 在&#x200B;**Settings**&#x200B;下，按一下&#x200B;**Marketo配置**。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >如果&#x200B;**Marketo配置**&#x200B;缺失，請嘗試刷新頁面。 如果問題持續存在，[請再次發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)，或嘗試登出並重新登入。

1. 按一下&#x200B;**Default**。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 按一下&#x200B;**Marketo用戶**&#x200B;欄位並選擇同步用戶。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 按一下右下角的![](assets/image2015-3-13-15-3a10-3a11.png)以儲存變更。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 按一下&#x200B;**發佈所有自定義**。

   ![](assets/publish-all-customizations1.png)

## 繼續執行步驟3 {#before-proceeding-to-step}之前

* 如果您想要限制同步的記錄數，[現在設定自訂同步篩選](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 運行[驗證Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)進程。 它會驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入「Marketo同步使用者」。

幹得好！

>[!MORELIKETHIS]
>
>[步驟3（共3步）:ConnectMarketo與Dynamics（2013年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
