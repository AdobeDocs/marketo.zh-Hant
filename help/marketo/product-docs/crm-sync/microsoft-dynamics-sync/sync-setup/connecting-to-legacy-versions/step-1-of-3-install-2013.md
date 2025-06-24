---
unique-page-id: 3571813
description: 步驟3之1 — 在Dynamics中安裝Marketo解決方案（2013內部部署） - Marketo檔案 — 產品檔案
title: 步驟3之1 — 在Dynamics中安裝Marketo解決方案（2013內部部署）
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 1%

---

# 步驟3之1：在Dynamics中安裝Marketo解決方案（2013內部部署） {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

在同步Microsoft Dynamics內部部署和Marketo Engage之前，您必須先在Dynamics中安裝Marketo解決方案。

>[!NOTE]
>
>將Marketo同步至CRM後，如果不取代執行個體，就無法執行新的同步。

>[!PREREQUISITES]
>
>您必須設定[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0、2.1或3.0 (ADFS)的[網際網路對向部署](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} (IFD)。 附註：當您按一下連結時，IFD檔案會自動下載。
>
>開始之前[請下載Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。

>[!NOTE]
>
>**需要Dynamics管理員許可權**。
>
>您需要CRM系統管理員許可權才能執行此同步處理。

1. 登入Dynamics 按一下&#x200B;**[!UICONTROL Microsoft Dynamics CRM]**&#x200B;下拉式功能表並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;下，選取&#x200B;**[!UICONTROL Solutions]**。

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 按一下「**[!UICONTROL Import]**」。

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 按一下&#x200B;**[!UICONTROL Browse]**&#x200B;並選取[下載的解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. 檢視方案資訊並按一下&#x200B;**[!UICONTROL View solution package details]**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 檢查完所有詳細資料後，按一下&#x200B;**[!UICONTROL Close]**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回[方案資訊]頁面，按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 確認勾選SDK選項。 按一下「**[!UICONTROL Import]**」。

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 下載記錄檔（如果您需要），然後按一下&#x200B;**[!UICONTROL Close]**。

   >[!NOTE]
   >
   >您可能會看到顯示「Marketo銷售機會管理已完成，但有警告」的訊息。 這是完全正常的情況。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo銷售機會管理現在會出現在&#x200B;**[!UICONTROL All Solutions]**&#x200B;頁面上。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. 選取Marketo解決方案並按一下&#x200B;**[!UICONTROL Publish all Customizations]**。

   ![](assets/image2014-12-11-10-3a41-3a32.png)

>[!CAUTION]
>
>停用任何Marketo SDK訊息程式會導致安裝中斷！

>[!MORELIKETHIS]
>
>[步驟2之3：設定Marketo （2013內部部署）的同步使用者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md){target="_blank"}
