---
unique-page-id: 37355600
description: 從您的MS Dynamics Instance - Marketo Docs —— 產品檔案解除安裝MSI
title: 從您的MS Dynamics Instance解除安裝MSI
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# 從您的MS Dynamics Instance解除安裝MSI {#uninstall-msi-from-your-ms-dynamics-instance}

若要從MS Dynamics例項中解除安裝MSI，您必須在Marketo和MS Dynamics中執行步驟。

>[!NOTE]
>
>**必要條件**
>
>[禁用全局MS Dynamics Sync](http://docs.marketo.com/x/TAA6Ag)

1. 在Marketo中，按一下「管 **理員**」。

   ![](assets/one-1.png)

1. 按一 **下Sales Insight**。

   ![](assets/six.png)

1. 按一下 **編輯欄位同步**。

   ![](assets/seven.png)

1. 選中「禁 **用同步** 」複選框，然後單 **擊「保存」**。

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >請務必先 [禁用全局MS動態同步](http://docs.marketo.com/x/TAA6Ag) ，然後再禁用欄位同步。

   ![](assets/eight.png)

## 在MS Dynamics實例中執行以下步驟： {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 按一下 **進階設定**。
1. 按一下 **解決方案**。
1. 選取 **Marketo Sales Insight** ，然後按一下刪除圖示。
1. 出現「Uninstall Solution（卸載解決方案）」模式時，按一下「 **OK（確定）**」。

   MS Dynamics解決方案通常需要20分鐘左右才能完全解除安裝。 不過，如果您有大型的MS Dynamics例項，可能需要更久的時間。

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >請記得在解除安裝MSI後，開啟全域MS Dynamics同步。

