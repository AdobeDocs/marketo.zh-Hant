---
unique-page-id: 37355600
description: 從您的MS [!DNL Dynamics] 執行個體解除安裝MSI - Marketo檔案 — 產品檔案
title: 從您的MS [!DNL Dynamics] 執行個體解除安裝MSI
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 3%

---

# 從您的MS [!DNL Dynamics]執行個體解除安裝MSI {#uninstall-msi-from-your-ms-dynamics-instance}

若要從MS [!DNL Dynamics]執行個體解除安裝MSI，您必須同時在Marketo和MS [!DNL Dynamics]中執行步驟。

>[!PREREQUISITES]
>
>[停用全域MS [!DNL Dynamics] 同步](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/one-1.png)

1. 按一下「**[!UICONTROL Sales Insight]**」。

   ![](assets/six.png)

1. 按一下「**[!UICONTROL Edit Field Sync]**」。

   ![](assets/seven.png)

1. 選取&#x200B;**[!UICONTROL Disable Sync]**&#x200B;核取方塊並按一下&#x200B;**[!UICONTROL Save]**。

   >[!NOTE]
   >
   >在停用欄位同步之前，請確定您[停用全域MS Dynamics同步處理](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)。

   ![](assets/eight.png)

## 下列步驟會在您的MS [!DNL Dynamics]執行個體中進行： {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 按一下「**[!UICONTROL Advanced Settings]**」。

1. 按一下「**[!UICONTROL Solutions]**」。

1. 選取&#x200B;**[!UICONTROL Marketo Sales Insight]**&#x200B;並按一下刪除圖示。

1. 當解除安裝方案強制回應視窗彈出時，請按一下&#x200B;**[!UICONTROL OK]**。

   MS [!DNL Dynamics]解決方案通常需要20分鐘才能完全解除安裝。 不過，如果您有大型MS [!DNL Dynamics]執行個體，則可能需要更長的時間。

   >[!NOTE]
   >
   >解除安裝MSI之後，請記得開啟全域MS [!DNL Dynamics]同步處理。
