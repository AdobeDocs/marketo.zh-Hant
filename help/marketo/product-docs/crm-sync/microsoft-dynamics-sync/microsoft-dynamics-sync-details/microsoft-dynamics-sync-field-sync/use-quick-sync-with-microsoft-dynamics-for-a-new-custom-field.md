---
unique-page-id: 10098379
description: 將與Microsoft Dynamics快速同步用於新自訂欄位 — Marketo檔案 — 產品檔案
title: 針對新自訂欄位使用「與Microsoft Dynamics快速同步」
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 1%

---

# 使用新自訂欄位的[與[!DNL Microsoft Dynamics]快速同步] {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

行銷或銷售人員想要新欄位。 或者，您可能在初始欄位選取中忘記了一項。 或者，您的需求已變更。 無論如何，您可以使用「快速同步」來重新同步特定欄位。

通常您會使用「快速同步」來新增欄位，並重新整理值。 但是，在某些情況下，您可能會想要同步現有欄位。 您可以根據更新或建立的日期範圍來限制欄位同步。 如需詳細資訊，請參閱下方的[進階同步選項](#Advanced_Sync_Options)。

快速同步可以同步Null值。 例如，如果您使用值A和B，並將[!DNL Dynamics]中的B值變更為null，則會將null值同步至Marketo。

## 所有記錄的快速同步 {#quick-sync-for-all-records}

以下說明如何使用「快速同步」來重新同步新欄位。

1. 在Marketo中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. 按一下「**[!UICONTROL Microsoft Dynamics]**」。

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. 在[!UICONTROL Field Sync Details]上，按一下&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. 選取要快速同步的欄位並按一下&#x200B;**[!UICONTROL Save]**。

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

1. 清除現有欄位的核取方塊。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. 再次開啟快顯視窗並重新選取欄位。

   ![](assets/select-field-reselect-hand.png)

1. 按一下「**[!UICONTROL Advanced Sync]**」。

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. 選擇&#x200B;**[!UICONTROL Updated]**&#x200B;並使用日期選擇器選取日期範圍。 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   只有在2016年8月19日到2016年9月19日之間更新的記錄才會在該欄位中進行「快速同步」。

## 修正不同步欄位 {#fixing-out-of-sync-fields}

在極少數情況下，[!DNL Dynamics]和Marketo欄位不同步，有一個快速輕鬆的方法可重新同步它們。

1. 取消選取欄位並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. 重新選取欄位並按一下&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   這應該能解決這個問題！
