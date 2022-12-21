---
unique-page-id: 37355600
description: 從您的MS Dynamics實例卸載MSI - Marketo文檔 — 產品文檔
title: 從MS Dynamics實例卸載MSI
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# 從MS Dynamics實例卸載MSI {#uninstall-msi-from-your-ms-dynamics-instance}

要從MS Dynamics實例卸載MSI，您需要在Marketo和MS Dynamics中執行步驟。

>[!PREREQUISITES]
>
>[禁用全局MS Dynamics同步](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. 在Marketo中，按一下 **管理**.

   ![](assets/one-1.png)

1. 按一下 **Sales Insight**.

   ![](assets/six.png)

1. 按一下 **編輯欄位同步**.

   ![](assets/seven.png)

1. 選取 **禁用同步** 核取方塊和按一下 **儲存**.

   >[!NOTE]
   >
   >確保 [禁用全局MS動態同步](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) 停用欄位同步之前。

   ![](assets/eight.png)

## 在MS Dynamics實例中執行以下步驟： {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 按一下 **進階設定**.

1. 按一下 **解決方案**.

1. 選擇 **Marketo Sales Insight** 並按一下刪除圖示。

1. 出現「Uninstall Solution（卸載解決方案）」強制回應時，按一下 **確定**.

   MS Dynamics解決方案要完全卸載通常需要20分鐘。 不過，如果您有大型MS Dynamics執行個體，則可能需要更久的時間。

   >[!NOTE]
   >
   >卸載MSI後，請記得開啟全局MS Dynamics同步。
