---
unique-page-id: 7504736
description: 安裝Marketo for Microsoft Dynamics 2015內部部署步驟1之3 - Marketo檔案 — 產品檔案
title: 安裝適用於Microsoft Dynamics 2015內部部署的Marketo步驟3之1
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# 步驟3之1：設定Marketo的同步使用者（2015年內部部署） {#step-of-configure-sync-user-for-marketo-on-premises-2015}

您必須先在Dynamics中安裝Microsoft Dynamics解決方案，才能將Marketo 2015內部部署與Marketo Engage同步。

>[!NOTE]
>
>將Marketo同步至CRM後，新CRM就無法同步至現有的Marketo執行個體。

>[!PREREQUISITES]
>
>如果您正在使用Microsoft Dynamics內部部署，則必須設定[網際網路對向部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD)及[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS)。 附註：當您按一下連結時，IFD檔案會自動下載。
>
>開始之前[請下載Marketo銷售機會管理解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}。

>[!NOTE]
>
>**需要Dynamics管理員許可權**。
>
>您需要CRM系統管理員許可權才能執行此同步處理。

1. 登入Dynamics。 按一下&#x200B;**[!UICONTROL Microsoft Dynamics CRM]**&#x200B;下拉式功能表，然後選取&#x200B;**[!UICONTROL 設定]**。

   ![](assets/image2015-3-19-8-33-29.png)

1. 在&#x200B;**[!UICONTROL 設定]**&#x200B;下，選取&#x200B;**[!UICONTROL 解決方案]**。

   ![](assets/image2015-3-19-8-33-3.png)

1. 按一下&#x200B;**[!UICONTROL 匯入]**。

   ![](assets/image2015-3-19-8-34-8.png)

1. 按一下&#x200B;**[!UICONTROL 瀏覽]**&#x200B;並選取您[下載的解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)。 按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/image2015-3-19-9-20-56.png)

1. 檢視方案資訊，然後按一下&#x200B;**[!UICONTROL 檢視方案封裝詳細資料]**。

   ![](assets/image2015-11-18-11-12-8.png)

1. 檢查完所有詳細資料後，按一下[關閉]。**&#x200B;**

   ![](assets/step6.png)

1. 返回[方案資訊]頁面，按一下[下一步]。**&#x200B;**

   ![](assets/image2015-3-19-9-21-50.png)

1. 確認已選取SDK選項核取方塊。 按一下&#x200B;**[!UICONTROL 匯入]**。

   ![](assets/image2015-3-19-9-19-12.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

   ![](assets/image2015-3-11-11-34-9.png)

1. 下載記錄檔（如果您需要），然後按一下&#x200B;**[!UICONTROL 關閉]**。

   >[!NOTE]
   >
   >您可能會看到顯示「Marketo銷售機會管理已完成，但有警告」的訊息。 這是完全正常的情況。

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo銷售機會管理現在會出現在&#x200B;**[!UICONTROL 所有解決方案]**&#x200B;頁面上。

   ![](assets/image2015-3-19-8-40-38.png)

1. 選取Marketo解決方案，然後按一下&#x200B;**[!UICONTROL Publish所有自訂]**。

   ![](assets/image2015-3-19-8-41-21.png)

   做得很好！安裝完成。

   >[!CAUTION]
   >
   >停用任何Marketo SDK傳訊程式會導致安裝中斷！

   >[!MORELIKETHIS]
   >
   >[安裝適用於Microsoft Dynamics 2015內部部署的Marketo步驟2 （共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md){target="_blank"}
