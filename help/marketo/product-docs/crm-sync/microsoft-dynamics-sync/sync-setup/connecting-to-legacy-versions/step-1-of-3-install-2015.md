---
unique-page-id: 7504736
description: 安裝適用於Microsoft Dynamics 2015的Marketo內部部署步驟1之3 - Marketo檔案 — 產品檔案
title: 安裝適用於Microsoft Dynamics 2015內部部署的Marketo步驟3之1
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 1%

---

# 步驟3之1：設定Marketo的同步使用者（2015年內部部署） {#step-of-configure-sync-user-for-marketo-on-premises-2015}

您必須先在[!DNL Microsoft Dynamics]中安裝Marketo解決方案，才能與Marketo同步[!DNL Dynamics] 2015內部部署。

>[!NOTE]
>
>將Marketo同步至CRM後，新CRM就無法同步至現有的Marketo執行個體。

>[!PREREQUISITES]
>
>如果您使用[!DNL Microsoft Dynamics]內部部署，則必須設定[網際網路對向部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD)及[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS)。 附註：當您按一下連結時，IFD檔案會自動下載。
>
>開始之前[請下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。

>[!NOTE]
>
>**需要Dynamics管理員許可權**。
>
>您需要CRM系統管理員許可權才能執行此同步處理。

1. 登入&#x200B;**[!DNL Dynamics]。**&#x200B;按一下&#x200B;**[!UICONTROL Microsoft Dynamics CRM]**&#x200B;下拉式功能表並選取&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2015-3-19-8-33-29.png)

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;下，選取&#x200B;**[!UICONTROL Solutions]**。

   ![](assets/image2015-3-19-8-33-3.png)

1. 按一下「**[!UICONTROL Import]**」。

   ![](assets/image2015-3-19-8-34-8.png)

1. 按一下&#x200B;**[!UICONTROL Browse]**&#x200B;並選取您[下載的解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 按一下「**[!UICONTROL Next]**」。

   ![](assets/image2015-3-19-9-20-56.png)

1. 檢視[!UICONTROL Solution Information]並按一下&#x200B;**[!UICONTROL View solution package details]**。

   ![](assets/image2015-11-18-11-12-8.png)

1. 檢查完所有詳細資料後，按一下&#x200B;**[!UICONTROL Close]**。

   ![](assets/step6.png)

1. 返回[!UICONTROL Solution Information]頁面，按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2015-3-19-9-21-50.png)

1. 確認已選取SDK選項核取方塊。 按一下「**[!UICONTROL Import]**」。

   ![](assets/image2015-3-19-9-19-12.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

   ![](assets/image2015-3-11-11-34-9.png)

1. 下載記錄檔（如果您需要），然後按一下&#x200B;**[!UICONTROL Close]**。

   >[!NOTE]
   >
   >您可能會看到顯示「Marketo銷售機會管理已完成，但有警告」的訊息。 這是完全正常的情況。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo銷售機會管理現在會出現在&#x200B;**[!UICONTROL All Solutions]**&#x200B;頁面上。

   ![](assets/image2015-3-19-8-40-38.png)

1. 選取Marketo解決方案並按一下&#x200B;**[!UICONTROL Publish All Customizations]**。

   ![](assets/image2015-3-19-8-41-21.png)

   做得很好！安裝完成。

   >[!CAUTION]
   >
   >停用任何Marketo SDK訊息程式會導致安裝中斷！

   >[!MORELIKETHIS]
   >
   >[為 [!DNL Microsoft Dynamics] 2015內部部署第2步（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)安裝Marketo
