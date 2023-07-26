---
unique-page-id: 10098379
description: 將與Microsoft Dynamics快速同步用於新自訂欄位 — Marketo檔案 — 產品檔案
title: 使用與Microsoft Dynamics快速同步處理新自訂欄位
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# 使用與Microsoft Dynamics快速同步處理新自訂欄位 {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

行銷或銷售人員想要新欄位。 或者，您可能在初始欄位選取中忘記了一項。 或者，您的需求已變更。 無論如何，您可以使用「快速同步」來重新同步特定欄位。

通常您會使用「快速同步」來新增欄位，並重新整理值。 但是，在某些情況下，您可能會想要同步現有欄位。 您可以根據更新或建立的日期範圍來限制欄位同步。 另請參閱 [進階同步選項](#Advanced_Sync_Options) 詳細資料請參閱下文。

快速同步可以同步Null值。 例如，如果您使用值A和B，並將Dynamics中的B值變更為null，則會將null值同步至Marketo。

## 所有記錄的快速同步 {#quick-sync-for-all-records}

以下說明如何使用「快速同步」來重新同步新欄位。

1. 在Marketo中，按一下 **管理員**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. 按一下 **Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. 在欄位同步詳細資訊上，按一下 **編輯**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. 選取要快速同步的欄位並按一下 **儲存**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >您可以從多個實體中選取欄位。

1. 同步完成後，您將會收到通知。

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >同步處理會與其他同步處理並排執行，而且視資料庫大小而定，可能需要很長時間才能完成。 當欄位在佇列中等待同步時，您無法取消選取它。

## 進階同步選項 {#advanced-sync-options}

如果您想要同步現有欄位，但只針對有限的資料集進行同步處理，該怎麼做？ 方法如下。

1. 清除現有欄位的核取方塊。 按一下 **儲存**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. 再次開啟快顯視窗並重新選取欄位。

   ![](assets/select-field-reselect-hand.png)

1. 按一下 **進階同步**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. 選擇 **已更新** 並使用日期選擇器選取日期範圍。 按一下 **儲存**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   只有在2016年8月19日到2016年9月19日之間更新的記錄才會在該欄位中進行「快速同步」。

## 修正不同步欄位 {#fixing-out-of-sync-fields}

在Dynamics和Marketo欄位不同步的罕見情況下，可以快速輕鬆地重新同步它們。

1. 取消選取欄位並按一下 **儲存**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. 重新選取欄位並按一下 **儲存**. 僅此而已！

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   這應該能解決這個問題！
