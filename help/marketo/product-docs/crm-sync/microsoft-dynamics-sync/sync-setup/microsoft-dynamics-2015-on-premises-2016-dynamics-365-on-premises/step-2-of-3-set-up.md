---
unique-page-id: 7504739
description: 安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟2（共3步）-行銷檔案——產品檔案
title: 安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟2（共3步）
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---


# 步驟2（共3步）

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 2 of 3-->

完成上述步驟的出色工作。 讓我們繼續過去。

>[!NOTE]
>
>**必要條件**
>
>* [安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟1（共3步）](step-1-of-3-install.md)

>



## 指派同步使用者角色 {#assign-sync-user-role}

將「Marketo同步使用者」角色僅指派給「Marketto同步使用者」。 您不需要將它指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo 4.0.0.14版及更新版本。 對於舊版，所有使用者都必須具有同步使用者角色。 若要升級您的Marketo，請參 [閱升級Microsoft Dynamics的Marketo解決方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在「設 **定**」下，按一 **下「保全」**。

   ![](assets/assign1.png)

1. 按一下「 **使用者**」。

   ![](assets/assign2.png)

1. 您會在這裡看到使用者清單。 選擇專用的Marketo Sync使用者，或連絡 [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理員以建立Marketo專用的使用者。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 按一下 **管理角色**。

   ![](assets/assign4.png)

   勾選「Marketto Sync User」（行銷人員同步使用者），然後按一下「OK」（確定）。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果您看不到此角色，請返回第1步(共3 [步)](step-1-of-3-install.md) ，然後匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新都 **不會** 同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

快搞定了！ 在移至下一篇文章之前，我們只有最後幾段設定。

1. 在「設 **定」下**，按一 **下「行銷人員設定」**。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果Marketo Config遺失，請嘗試重新整理頁面。 如果問題持續發 [生，請發佈Marketo Solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) ，或嘗試登出並重新登入。

1. 按一下 **預設**。

   ![](assets/configure2.png)

1. 按一下「 **Marketto使用者** 」欄位，並選取同步使用者。

   ![](assets/configure3.png)

1. 按一下右下角的儲存圖示。

   ![](assets/configure4.png)

1. 按一 **下「發佈所有自訂」**。

   ![](assets/publish-all-customizations1.png)

## 繼續步驟3之前 {#before-proceeding-to-step}

* 如果您想要限制同步的記錄數，請立 [即設定自訂同步篩選](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 。
* 運行驗 [證Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) (Validate Microsoft Dynamics Sync)流程。 它會驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入Marketo同步使用者。

>[!NOTE]
>
>**相關文章**
>
>[安裝Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步驟3（共3步）](step-3-of-3-connect.md)
