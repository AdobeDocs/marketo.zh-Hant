---
unique-page-id: 7504739
description: 安裝Marketo for Microsoft Dynamics 2015內部部署步驟2之3 - Marketo檔案 — 產品檔案
title: 安裝適用於Microsoft Dynamics 2015內部部署的Marketo步驟3之2
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# 步驟3之2：設定Marketo for Dynamics （2015內部部署）{#step-of-set-up-for-marketo-on-premises-2015}

完成上述步驟的絕佳工作。 讓我們繼續討論這個問題。

>[!PREREQUISITES]
>
>[安裝適用於Microsoft Dynamics 2015內部部署的Marketo步驟1 （共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}

## 指派同步使用者角色 {#assign-sync-user-role}

僅將Marketo同步使用者角色指派給Marketo同步使用者。 您不需要將其指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo 4.0.0.14版和更新版本。 對於舊版，所有使用者都必須擁有同步使用者角色。 若要升級Marketo，請參閱[升級Microsoft Dynamics的Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}。

>[!IMPORTANT]
>
>同步處理使用者[的語言設定應該設定為英文](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}。

1. 在&#x200B;**[!UICONTROL 設定]**&#x200B;下，按一下&#x200B;**[!UICONTROL 安全性]**。

   ![](assets/assign1.png)

1. 按一下&#x200B;**[!UICONTROL 使用者]**。

   ![](assets/assign2.png)

1. 您將會在這裡看到使用者清單。 選取專用的Marketo Sync使用者，或連絡您的[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS)系統管理員，為Marketo建立專用使用者。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選取同步使用者。 按一下&#x200B;**[!UICONTROL 管理角色]**。

   ![](assets/assign4.png)

1. 檢查Marketo同步使用者，然後按一下&#x200B;**[!UICONTROL 確定]**。

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >同步使用者應該要有Marketo設定的讀取許可權。

   >[!TIP]
   >
   >如果您沒有看到角色，請返回3[&#128279;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}的步驟1並匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中所做的任何更新將&#x200B;_不會_&#x200B;同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

即將完成！ 在前往下一篇文章之前，我們僅有最後幾項的設定。

1. 在&#x200B;**[!UICONTROL 設定]**&#x200B;下，按一下&#x200B;**[!UICONTROL Marketo設定]**。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo設定，請嘗試重新整理頁面。 如果問題仍然存在，請[發佈Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}，或嘗試登出再重新登入。

1. 按一下&#x200B;**[!UICONTROL 預設]**。

   ![](assets/configure2.png)

1. 按一下&#x200B;**[!UICONTROL Marketo使用者]**&#x200B;欄位並選取同步使用者。

   ![](assets/configure3.png)

1. 按一下右下角的儲存圖示。

   ![](assets/configure4.png)

1. 按一下&#x200B;**[!UICONTROL Publish所有自訂]**。

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >同步使用者應該要有Marketo設定的讀取許可權。

## 繼續進行步驟3之前 {#before-proceeding-to-step}

* 若要限制同步處理的記錄數目，請立即[設定自訂同步處理篩選器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}。
* 執行[驗證Microsoft Dynamics同步處理](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}程式。 它可驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入Marketo Sync User。

>[!MORELIKETHIS]
>
>[安裝適用於Microsoft Dynamics 2015內部部署的Marketo步驟3之3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md){target="_blank"}
