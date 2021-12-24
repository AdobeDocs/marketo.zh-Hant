---
description: Install Marketo for Microsoft Dynamics 2016/Dynamics 365 On-Premises 1 of 3 - Marketo Docs - Product Documentation
title: Install Marketo for Microsoft Dynamics 2016/Dynamics 365 On-Premises Step 1 of 3
source-git-commit: 7b1f0d0d45bbfe3d8b781282e0a4ef1884a2bf40
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Step 1 of 3: Configure Sync User for Marketo (2016 On-Prem /Dynamics 365 On-Premises) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

您必須先在Dynamics中安裝Microsoft解決方案，才能將Dynamics 2015內部部署或2016(Dynamics 365)與Marketo同步。

>[!NOTE]
>
>將Marketo同步至CRM後，無法將新CRM同步至現有的Marketo例項。

>[!PREREQUISITES]
>
>如果您使用Microsoft Dynamics On-Premise，您必須 [面向Internet的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)與 [Active Directory聯合身份驗證服務](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+(ADFS)已配置。 Note: The IFD document downloads automatically when you click the link.
>
>[下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 開始之前。

>[!NOTE]
>
>**需要Dynamics管理員權限。**
>
>您需要CRM管理員權限才能執行此同步。

1. Log in to **Dynamics.** 按一下 **Microsoft Dynamics CRM** 下拉式功能表，然後選取 **設定**.

   ![](assets/image2015-3-19-8-33-29.png)

1. 在 **設定**，選取 **解決方案**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Click **Import**.

   ![](assets/image2015-3-19-8-34-8.png)

1. 按一下 **瀏覽** 並選擇您的解決方案 [已下載](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Click **Next**.

   ![](assets/image2015-3-19-9-20-56.png)

1. 檢視解決方案資訊，然後按一下 **查看解決方案包詳細資訊**.

   ![](assets/image2015-11-18-11-12-8.png)

1. 檢查完所有詳細資訊後，按一下 **關閉**.

   ![](assets/step6.png)

1. 返回「解決方案資訊」頁面，按一下 **下一個**.

   ![](assets/image2015-3-19-9-21-50.png)

1. 確認已選取SDK選項核取方塊。 按一下 **匯入**.

   ![](assets/image2015-3-19-9-19-12.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >You will need to enable pop-ups on your browser to complete the installation process.

   ![](assets/image2015-3-11-11-34-9.png)

1. Download a log file (if you want) and click **Close**.

   >[!NOTE]
   >
   >您可能會看到一則訊息，指出「Marketo銷售機會管理已完成並出現警告」。 This is fully expected.

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management現在會顯示在 **所有解決方案** 頁面。

   ![](assets/image2015-3-19-8-40-38.png)

1. Select the Marketo solution and click **Publish All Customizations**.

   ![](assets/image2015-3-19-8-41-21.png)

   五！ The installation is finished.

   >[!CAUTION]
   >
   >停用任何Marketo SDK傳訊程式都會導致安裝中斷！

   >[!MORELIKETHIS]
   >
   >[安裝Dynamics 2015內部部署和2016 365內部部署的Marketo步驟2（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
