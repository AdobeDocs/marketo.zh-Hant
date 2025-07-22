---
unique-page-id: 3571805
description: 步驟3之1 — 安裝Marketo解決方案（2011年內部部署） - Marketo檔案 — 產品檔案
title: 步驟3之1 — 安裝Marketo解決方案（2011年內部部署）
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 1%

---

# 步驟3之1：安裝Marketo解決方案（2011年內部部署） {#step-of-install-the-marketo-solution-on-premises}

在同步處理[!DNL Microsoft Dynamics]內部部署與Marketo之前，您必須先在[!DNL Dynamics]中安裝Marketo解決方案。

>[!NOTE]
>
>將Marketo同步至CRM後，如果不取代執行個體，就無法執行新的同步。

>[!PREREQUISITES]
>
>您必須設定[Active Directory Federation Services](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} 2.0、2.1或3.0 (ADFS)的[網際網路對向部署](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (IFD)。 **附註**：當您按一下連結時，IFD檔案會自動下載。
>
>開始之前[請下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。

>[!NOTE]
>
>需要&#x200B;**[!DNL Dynamics]個管理員許可權。**
>
>您需要CRM系統管理員許可權才能執行此同步處理。

1. 登入&#x200B;**[!DNL Dynamics]**，在左下方功能表中選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. 在樹狀結構中選取&#x200B;**[!UICONTROL Solutions]**。

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. 按一下「**[!UICONTROL Import]**」。

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. 按一下&#x200B;**[!UICONTROL Browse]**。 選取您[下載的Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. 檢視方案資訊並按一下&#x200B;**[!UICONTROL View solution package details]**。

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 檢查完所有詳細資料後，按一下&#x200B;**[!UICONTROL Close]**。

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回[方案資訊]頁面，按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. 確認勾選SDK訊息選項核取方塊。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

1. 現在請等待匯入完成。 站起來做一些伸展。

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. 按一下「**[!UICONTROL Close]**」。

   >[!NOTE]
   >
   >您可能會看到顯示「Marketo銷售機會管理已完成，但有警告」的訊息。 這是完全正常的情況。

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. [!UICONTROL Marketo Lead Management]現在會顯示在&#x200B;**[!UICONTROL All Solutions]**&#x200B;頁面上。

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. 選取[!UICONTROL Marketo Lead Management]並按一下&#x200B;**[!UICONTROL Publish All Customizations]**。

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>停用任何Marketo SDK訊息程式會導致安裝中斷！

>[!MORELIKETHIS]
>
>[步驟2 （共3步）：在 [!DNL Dynamics] （2011年內部部署）中設定Marketo同步使用者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)
