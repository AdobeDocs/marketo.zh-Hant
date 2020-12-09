---
unique-page-id: 3571816
description: 第2步（共3步）-為行銷人員設定同步使用者（2013年內部部署）-行銷人員檔案——產品檔案
title: 步驟2（共3步）-為Marketo設定同步使用者（2013年內部部署）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# 步驟2（共3步）:為Marketo設定同步使用者（2013年內部部署） {#step-of-configure-sync-user-for-marketo-on-premises}

完成前述步驟的出色工作，讓我們繼續進行。

>[!PREREQUISITES]
>
>* [步驟1（共3步）:在Dynamics中安裝Marketo解決方案（2013年內部部署）](step-1-of-3-install.md)


## 指派同步使用者角色 {#assign-sync-user-role}

將「Marketo同步使用者」角色僅指派給「Marketto同步使用者」。 您不需要將它指派給任何其他使用者。

>[!NOTE]
>
>這適用於Marketo增效模組4.0.0.14版及更新版本。 對於舊版，所有使用者都必須具有同步使用者角色。 若要升級Marketo，請參 [閱升級Microsoft Dynamics的Marketo解決方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在「設 **定**」下，按一 **下「管理」**。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 選擇 **用戶**。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您會在這裡看到使用者清單。 選擇您專用的Marketo Sync使用者，或連絡 [Active Directory Federation Services(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx)[管理員以建立專用於Marketo的新使用者。](http://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 選擇同步用戶。 按一下並 ![](assets/image2015-3-26-11-3a16-3a22.png)選擇管 **理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 勾選「 **Marketto同步使用者」** ，然後按一 **下「確定」**。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >如果您看不到此角色，請返回第1步(共3 [步)](step-1-of-3-install.md) ，然後匯入解決方案。

   >[!NOTE]
   >
   >同步使用者在您的CRM中進行的任何更新都 **不會** 同步回Marketo。

## 設定Marketo解決方案 {#configure-marketo-solution}

快搞定了！ 在移至下一篇文章之前，我們只有最後幾段設定。

1. 在「設 **定」下**，按一 **下「行銷人員設定」**。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >如果 **Marketo Config遺失** ，請嘗試重新整理頁面。 如果問題持續發 [生，請再次發佈Marketo解決方案](https://docs.marketo.com/pages/viewpage.action?pageId=3571813#Step1of3:InstalltheMarketoSolutioninDynamics(2013On-Premises)-PublishAllCustomizations) ，或嘗試登出並重新登入。

1. 按一下 **預設**。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 按一下「 **Marketto使用者** 」欄位，並選取同步使用者。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 按一 ![](assets/image2015-3-13-15-3a10-3a11.png) 下右下角的以儲存變更。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 按一 **下「發佈所有自訂」**。

   ![](assets/publish-all-customizations1.png)

## 繼續步驟3之前 {#before-proceeding-to-step}

* 如果您想要限制同步的記錄數，請立 [即設定自訂同步篩選](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 。
* 運行驗 [證Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) (Validate Microsoft Dynamics Sync)流程。 它會驗證您的初始設定是否正確完成。
* 在Microsoft Dynamics CRM中登入Marketo同步使用者。

幹得好！

>[!NOTE]
>
>**相關文章**
>
>* [步驟3（共3步）:Connect Marketo與Dynamics（2013年內部部署）](step-3-of-3-connect.md)

