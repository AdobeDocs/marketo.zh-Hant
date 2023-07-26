---
unique-page-id: 37355600
description: 從MS Dynamics執行個體解除安裝MSI - Marketo檔案 — 產品檔案
title: 從MS Dynamics執行個體解除安裝MSI
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# 從MS Dynamics執行個體解除安裝MSI {#uninstall-msi-from-your-ms-dynamics-instance}

若要從MS Dynamics執行個體解除安裝MSI，您需要在Marketo和MS Dynamics中執行步驟。

>[!PREREQUISITES]
>
>[停用全域MS Dynamics同步處理](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. 在Marketo中，按一下 **管理員**.

   ![](assets/one-1.png)

1. 按一下 **銷售分析**.

   ![](assets/six.png)

1. 按一下 **編輯欄位同步**.

   ![](assets/seven.png)

1. 選取 **停用同步** 核取方塊並按一下 **儲存**.

   >[!NOTE]
   >
   >請確定 [停用全域MS Dynamics同步處理](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) 在停用欄位同步處理之前。

   ![](assets/eight.png)

## 下列步驟會在您的MS Dynamics執行個體中進行： {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 按一下 **進階設定**.

1. 按一下 **解決方案**.

1. 選取 **Marketo Sales Insight** 並按一下刪除圖示。

1. 當解除安裝解決方案強制回應視窗彈出時，請按一下 **確定**.

   MS Dynamics解決方案通常需要大約20分鐘才能完全解除安裝。 不過，如果您有大型MS Dynamics執行個體，則可能需要更長的時間。

   >[!NOTE]
   >
   >解除安裝MSI之後，請記得開啟全域MS Dynamics同步處理。
