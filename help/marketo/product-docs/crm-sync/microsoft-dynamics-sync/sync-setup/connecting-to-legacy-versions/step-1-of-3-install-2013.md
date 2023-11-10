---
unique-page-id: 3571813
description: 步驟3之1 — 在Dynamics中安裝Marketo解決方案（2013內部部署） - Marketo檔案 — 產品檔案
title: 步驟3之1 — 在Dynamics中安裝Marketo解決方案（2013內部部署）
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 步驟3之1：在Dynamics中安裝Marketo解決方案（2013內部部署） {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

在同步Microsoft Dynamics內部部署和Marketo Engage之前，您必須先在Dynamics中安裝Marketo解決方案。

>[!NOTE]
>
>將Marketo同步至CRM後，如果不取代執行個體，就無法執行新的同步。

>[!PREREQUISITES]
>
>您必須擁有 [網際網路對向部署](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) with [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 已設定2.0、2.1或3.0 (ADFS)。 附註：當您按一下連結時，IFD檔案會自動下載。
>
>[下載Marketo解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} 開始之前。

>[!NOTE]
>
>**需要Dynamics管理員許可權**.
>
>您需要CRM系統管理員許可權才能執行此同步處理。

1. 登入Dynamics 按一下 **[!UICONTROL Microsoft Dynamics CRM]** 下拉式功能表並選取 **[!UICONTROL 設定]**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. 在 **[!UICONTROL 設定]**，選取 **[!UICONTROL 解決方案]**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. 按一下 **[!UICONTROL 匯入]**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. 按一下 **[!UICONTROL 瀏覽]** 並選取 [下載的解決方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. 按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. 檢視解決方案資訊，然後按一下 **[!UICONTROL 檢視解決方案套件詳細資料]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. 檢查完所有詳細資料後，按一下 **[!UICONTROL 關閉]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. 返回「解決方案資訊」頁面，按一下 **[!UICONTROL 下一個]**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. 請確定已勾選SDK選項。 按一下 **[!UICONTROL 匯入]**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. 等待匯入完成。

   >[!TIP]
   >
   >您必須啟用瀏覽器上的快顯視窗，才能完成安裝程式。

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. 下載記錄檔（如果您需要），然後按一下 **[!UICONTROL 關閉]**.

   >[!NOTE]
   >
   >您可能會看到顯示「Marketo銷售機會管理已完成，但有警告」的訊息。 這是完全正常的情況。

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo銷售機會管理現在會出現在 **[!UICONTROL 所有解決方案]** 頁面。

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. 選取Marketo解決方案並按一下 **[!UICONTROL 發佈所有自訂]**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

>[!CAUTION]
>
>停用任何Marketo SDK傳訊程式會導致安裝中斷！

>[!MORELIKETHIS]
>
>[步驟3之2：設定Marketo的同步使用者（2013內部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md){target="_blank"}
