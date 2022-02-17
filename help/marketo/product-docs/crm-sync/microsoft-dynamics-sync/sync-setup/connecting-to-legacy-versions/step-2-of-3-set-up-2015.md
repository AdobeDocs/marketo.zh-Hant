---
unique-page-id: 7504739
description: 安裝Marketo用於MicrosoftDynamics 2015內部部署步驟2（共3步） — Marketo文檔 — 產品文檔
title: 為MicrosoftDynamics 2015安裝Marketo內部部署步驟2（共3步）
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 19c568cdc3d31d07e42e99eb7e48f10a017b44f9
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 第2步（共3步）建立Marketo動力學（2015年啟動）{#step-of-set-up-for-marketo-on-premises-2015}

完成前面步驟的工作非常出色。 我們繼續過去。

>[!PREREQUISITES]
>
>[為MicrosoftDynamics 2015安裝Marketo內部部署步驟1（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)

## 分配同步用戶角色 {#assign-sync-user-role}

將「Marketo同步用戶」角色僅分配給「Marketo同步」用戶。 您不需要將其分配給任何其他用戶。

>[!NOTE]
>
>這適用於Marketo4.0.0.14版及更高版本。 對於早期版本，所有用戶必須具有同步用戶角色。 要升級您的Marketo，請參閱 [升級MarketoMicrosoft動力解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

>[!IMPORTANT]
>
>同步用戶的語言設定 [應設定為英語](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)。

1. 下 **設定**&#x200B;按一下 **安全**。

   ![](assets/assign1.png)

1. 按一下 **用戶**。

   ![](assets/assign2.png)

1. 您將在此處看到用戶清單。 選擇專用的Marketo同步用戶或與 [Active Directory聯合身份驗證服務](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理員為Marketo建立專用用戶。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 按一下 **管理角色**。

   ![](assets/assign4.png)

1. 檢查Marketo同步用戶，然後按一下 **確定**。

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >同步用戶應具有對Marketo配置的讀取權限。

   >[!TIP]
   >
   >如果看不到角色，請返回 [第1步（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) 並導入解決方案。

   >[!NOTE]
   >
   >同步用戶在您的CRM中所做的任何更新將 **不** 同步回Marketo。

## 配置Marketo解決方案 {#configure-marketo-solution}

快好了！ 我們只有最後幾個配置，然後再轉到下一篇文章。

1. 下 **設定**&#x200B;按一下 **Marketo配置**。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo配置，請嘗試刷新頁面。 如果問題仍然存在， [發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) 或者嘗試註銷並重新登錄。

1. 按一下 **預設**。

   ![](assets/configure2.png)

1. 按一下 **Marketo用戶** ，然後選擇同步用戶。

   ![](assets/configure3.png)

1. 按一下右下角的保存表徵圖。

   ![](assets/configure4.png)

1. 按一下 **發佈所有自定義項**。

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >同步用戶應具有對Marketo配置的讀取權限。

## 繼續步驟3之前 {#before-proceeding-to-step}

* 如果要限制同步的記錄數， [設定自定義同步篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 現在。
* 運行 [驗證MicrosoftDynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 處理。 它驗證初始設定是否正確。
* 登錄到MarketoDynamics CRM中的Microsoft同步用戶。

>[!MORELIKETHIS]
>
>[為MicrosoftDynamics 2015安裝Marketo內部部署步驟3（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md)
