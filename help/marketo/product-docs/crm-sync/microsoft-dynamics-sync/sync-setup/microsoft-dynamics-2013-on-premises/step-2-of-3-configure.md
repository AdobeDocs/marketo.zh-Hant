---
unique-page-id: 3571816
description: 第2步（共3步） — 為Marketo配置同步用戶（2013年內部部署） — Marketo文檔 — 產品文檔
title: 第2步（共3步） — 為Marketo配置同步用戶（2013年內部部署）
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 第2步（共3步）:為Marketo配置同步用戶（2013年本地）{#step-of-configure-sync-user-for-marketo-on-premises}

完成上述步驟非常好，讓我們繼續完成。

>[!PREREQUISITES]
[第1步（共3步）:在Dynamics（2013內部部署）中安裝Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)>
>

## 分配同步用戶角色{#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
這適用於Marketo外掛程式4.0.0.14版和更新版本。 對於較舊版本，所有使用者都必須具有同步使用者角色。 若要升級Marketo，請參閱[升級Microsoft Dynamics適用的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

>[!IMPORTANT]
同步用戶[的語言設定應設定為English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)。

1. 在「**設定**」下，按一下「**管理**」。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 選擇&#x200B;**用戶**。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您會在此處看到使用者清單。 選擇您的專用Marketo同步用戶，或聯繫您的[Active Directory聯合身份驗證服務(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理員以建立專用於Marketo的新用戶。](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 按一下![](assets/image2015-3-26-11-3a16-3a22.png)並選擇&#x200B;**管理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 檢查&#x200B;**Marketo同步用戶**，然後按一下&#x200B;**確定**。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   如果您沒有看見角色，請返回至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)的[步驟1並匯入解決方案。

   >[!NOTE]
   同步使用者在您的CRM中進行的任何更新都會&#x200B;**not**&#x200B;同步回Marketo。

## 配置Marketo解決方案{#configure-marketo-solution}

快完成了！ 我們只有最後幾段配置，然後再轉到下一篇文章。

1. 在「**設定**」下，按一下「**Marketo設定**」。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   如果缺少&#x200B;**Marketo設定**，請嘗試重新整理頁面。 如果問題持續存在，請再次[發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)或嘗試登出再登入。

1. 按一下&#x200B;**預設**。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 按一下&#x200B;**Marketo User**&#x200B;欄位並選取同步使用者。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 按一下右下角的![](assets/image2015-3-13-15-3a10-3a11.png)以儲存變更。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 按一下「**發佈所有自定義項**」。

   ![](assets/publish-all-customizations1.png)

## 繼續執行步驟3之前{#before-proceeding-to-step}

* 如果要限制同步的記錄數，請立即[設定自定義同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 運行[驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)進程。 它會驗證您的初始設定是否正確執行。
* 在Microsoft Dynamics CRM中登入Marketo同步使用者。

幹得好！

>[!MORELIKETHIS]
[第3步（共3步）:連接Marketo和Dynamics（2013年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
