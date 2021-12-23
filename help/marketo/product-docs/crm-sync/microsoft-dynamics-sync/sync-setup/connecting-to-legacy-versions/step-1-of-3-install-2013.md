---
unique-page-id: 3571813
description: 第1步（共3步） — 在Dynamics中安裝Marketo解決方案（2013年內部部署） — Marketo檔案 — 產品檔案
title: 第1步（共3步） — 在Dynamics（2013年內部部署）中安裝Marketo解決方案
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 第1步（共3步）:在Dynamics（2013內部部署）中安裝Marketo解決方案 {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

您必須先在Dynamics中安裝Microsoft解決方案，才能同步Marketo Dynamics內部部署和Marketo。

>[!NOTE]
>
>將Marketo同步至CRM後，若不取代執行個體，就無法執行新同步。

>[!PREREQUISITES]
>
>您必須 [面向Internet的部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)與 [Active Directory聯合身份驗證服務](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0、2.1或3.0(ADFS)。 注意：當您按一下連結時，IFD文檔會自動下載。
>
>[下載Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 開始之前。

>[!NOTE]
>
>**需要Dynamics管理員權限。**
>
>您需要CRM管理員權限才能執行此同步。

1. 登入 **動態**. 按一下 **Microsoft Dynamics CRM** 下拉式功能表，然後選取 **設定**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 在 **設定**，選取 **解決方案**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 按一下 **匯入**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 按一下 **瀏覽** ，然後選取 [下載解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). 按一下 **下一個**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. 檢視解決方案資訊，然後按一下 **查看解決方案包詳細資訊**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 檢查完所有詳細資訊後，按一下 **關閉**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回「解決方案資訊」頁面，按一下 **下一個**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 確認已勾選SDK選項。 按一下 **匯入**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 下載記錄檔（如果需要），然後按一下 **關閉**.

   >[!NOTE]
   >
   >您可能會看到一則訊息，指出「Marketo銷售機會管理已完成並出現警告」。 這是完全預期的。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management現在會顯示在 **所有解決方案** 頁面。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. 選取Marketo解決方案，然後按一下 **發佈所有自訂**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

是不是太糟了？ 來吧，我會帶你過去。

>[!CAUTION]
>
>停用任何Marketo SDK傳訊程式都會導致安裝中斷！

>[!MORELIKETHIS]
>
>[第2步（共3步）:為Marketo配置同步用戶（2013年內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)
