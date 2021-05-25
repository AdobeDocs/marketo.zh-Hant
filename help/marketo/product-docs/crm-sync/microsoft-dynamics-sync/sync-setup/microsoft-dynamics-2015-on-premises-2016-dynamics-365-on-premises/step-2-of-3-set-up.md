---
unique-page-id: 7504739
description: 安裝Dynamics 2015內部部署和2016 365內部部署步驟2（共3步） — Marketo檔案 — 產品檔案
title: 安裝Dynamics 2015內部部署和2016 365內部部署的Marketo步驟2（共3步）
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 第2步（共3步）設定Dynamics Marketo（2015 On-Prem和2016 365 On-Prem）{#step-of-set-up-for-marketo-on-premises-and-365}

完成前述步驟非常好。 讓我們繼續過去。

>[!PREREQUISITES]
[安裝Dynamics 2015內部部署和2016 365內部部署的Marketo步驟1（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)>
>

## 分配同步用戶角色{#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
這適用於Marketo 4.0.0.14版和更新版本。 對於較舊版本，所有使用者都必須具有同步使用者角色。 若要升級您的Marketo，請參閱[升級Microsoft Dynamics適用的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

>[!IMPORTANT]
同步用戶[的語言設定應設定為English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)。

1. 在「**設定**」下，按一下「**安全**」。

   ![](assets/assign1.png)

1. 按一下「**用戶**」。

   ![](assets/assign2.png)

1. 您會在此處看到使用者清單。 選擇專用的Marketo同步用戶，或聯繫您的[Active Directory聯合身份驗證服務](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理員以為Marketo建立專用用戶。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 按一下「**管理角色**」。

   ![](assets/assign4.png)

   檢查Marketo同步用戶，然後按一下確定。

   ![](assets/assign5.png)

   >[!TIP]
   如果您沒有看見角色，請返回至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)的[步驟1並匯入解決方案。

   >[!NOTE]
   同步使用者在您的CRM中進行的任何更新都會&#x200B;**not**&#x200B;同步回Marketo。

## 配置Marketo解決方案{#configure-marketo-solution}

快完成了！ 我們只有最後幾段配置，然後再轉到下一篇文章。

1. 在「**設定**」下，按一下「**Marketo設定**」。

   ![](assets/configure1.png)

   >[!NOTE]
   如果缺少Marketo設定，請嘗試重新整理頁面。 如果問題持續存在，請[發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)或嘗試登出再登入。

1. 按一下&#x200B;**預設**。

   ![](assets/configure2.png)

1. 按一下&#x200B;**Marketo User**&#x200B;欄位並選取同步使用者。

   ![](assets/configure3.png)

1. 按一下右下角的儲存圖示。

   ![](assets/configure4.png)

1. 按一下「**發佈所有自定義項**」。

   ![](assets/publish-all-customizations1.png)

## 繼續執行步驟3之前{#before-proceeding-to-step}

* 如果要限制同步的記錄數，請立即[設定自定義同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 運行[驗證Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)進程。 它會驗證您的初始設定是否正確執行。
* 在Microsoft Dynamics CRM中登入Marketo同步使用者。

>[!MORELIKETHIS]
[安裝Dynamics 2015內部部署和2016 365內部部署的Marketo步驟3（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
