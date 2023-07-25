---
description: 傳送清單至廣告網路 — Marketo檔案 — 產品檔案
title: 傳送清單至廣告網路
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 傳送清單至廣告網路 {#send-a-list-to-an-ad-network}

瞭解如何將靜態清單傳送至LinkedIn、Facebook或Google。

## 如何傳送清單 {#how-to-send-a-list}

1. 在Marketo中選取您的清單，按一下 **清單動作** 下拉式清單，然後選取 **傳送至Ad Network**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. 在LinkedIn、Facebook或Google之間選擇（其他選專案前無法使用）。 在此範例中，我們選擇 **linkedIn**. 按一下 **下一個**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. 按一下「對象」下拉式清單，然後選取您需要的對象。

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >如果您需要檢查，可以透過「狀態」索引標籤檢視清單同步到的目標對象。

1. 選擇所需的推播型別，然後按一下 **更新**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >如果您選取「啟用連續對象同步」，Marketo會在Marketo執行個體中的清單變更時，保持所選廣告網路中的清單最新。 我們兩個都新增 **和** 從受眾中移除人員（如果他們從靜態清單中新增/移除）。

1. 就是這樣！ 按一下 **確定** 以結束。

   ![](assets/send-a-list-to-an-ad-network-5.png)

## 常見問題集 {#faq}

**單一靜態清單可以與多個廣告對象同步嗎？**

否，清單只能同步至單一目的地對象。

**如果我啟用與現有廣告對象的連續同步，現有對象是否會遭到取代？**

否，現有對象將會新增至，而非取代。
