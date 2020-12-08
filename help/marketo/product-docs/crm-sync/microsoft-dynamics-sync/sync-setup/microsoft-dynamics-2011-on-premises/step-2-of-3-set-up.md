---
unique-page-id: 3571807
description: 步驟2（共3步）-設定Marketo Sync User in Dynamics（2011年內部部署）- Marketo Docs —— 產品檔案
title: 第2步（共3步）-設定Marketo在Dynamics中同步使用者（2011年內部部署）
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---


# 步驟2（共3步）:在Dynamics中設定Marketto同步使用者（2011年內部部署） {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

完成前述步驟的出色工作，讓我們繼續進行。

>[!NOTE]
>
>**必要條件**
>
>* [步驟1（共3步）:安裝Marketo解決方案（2011年內部部署）](step-1-of-3-install.md)

>



## 指派同步使用者角色 {#assign-sync-user-role}

將「Marketo同步使用者」角色僅指派給「Marketto同步使用者」。 您不需要將它指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo增效模組4.0.0.14版及更新版本。 對於舊版，所有使用者都必須具有同步使用者角色。 若要升級Marketo，請參 [閱升級Microsoft Dynamics的Marketo解決方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在左下角的功能表中，選取「設 **定」**。

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. 在樹中，選擇「管 **理」**。

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. 選擇 **用戶**。

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. 您會在這裡看到使用者清單。 選擇您的專用Market以同步使用者，或連絡 [Active Directory Federation Services(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 管理員以建立專用於Marketo的新使用者。 按一下 **管理角色**。

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. 勾選「 **Marketto同步使用者」** ，然後按一 **下「確定」**。

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >如果您看不到此角色，請返回第1步(共3 [步)](step-1-of-3-install.md) ，然後匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新都 **不會** 同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

快搞定了！ 在移至下一篇文章之前，我們只有最後幾段設定。

1. 選擇 **設定**。 然後在樹狀結構中選取「**Marketo Config **」。

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >如果Marketo Config遺失，請嘗試重新整理頁面。 如果問題持續發 [生，請再次發佈Marketo解決方案](step-1-of-3-install.md) ，或登出並重新登入。

1. 按一下 **預設**。

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. 按一下 ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. 在彈出式選單中，選取同步使用者。 然後按一 **下確定**。

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. 按一 **下「儲存** 」以儲存變更。

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. 按一 **下「發佈所有自訂」**。

   ![](assets/publish-all-customizations1.png)

## 繼續步驟3之前 {#before-proceeding-to-step}

    *如果您想要限制同步的記錄數，請立即[設定自訂同步篩選](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
    *執行[驗證Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)程式。 它會驗證您的初始設定是否正確完成。
    *在Microsoft Dynamics CRM中登入Marketo同步使用者。

幹得好！

>[!NOTE]
>
>**相關文章**
>
>[步驟3（共3步）:將Microsoft Dynamics與Marketo連接（2011年內部部署）](step-3-of-3-connect.md)

