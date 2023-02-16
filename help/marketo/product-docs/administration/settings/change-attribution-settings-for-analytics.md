---
unique-page-id: 2360217
description: 變更Analytics的歸因設定 — Marketo檔案 — 產品檔案
title: 變更Analytics的歸因設定
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# 變更Analytics的歸因設定 {#change-attribution-settings-for-analytics}

您可以變更Marketo將聯絡人系結至首次接觸和多次接觸歸因商機的方式、潛在客戶轉換量度，以及行銷影響的商機標幟。

這些設定會影響 [計畫機會分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [機會分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)、和銷售機會分析區域。 這也會影響Program Analyzer報表。

1. 前往 **管理** 的上界。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 按一下 **收入週期分析**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 按一下 **編輯** 連結 **歸因**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >變更此設定不會修改任何Marketo資料；它只會變更報表的執行方式。 可隨時還原。

1. 選取選項，然後按一下 **儲存**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**明確**:僅具有角色的聯繫人（預設）。
   >
   >**混合**:具有角色的聯繫人（如果可用）。 如果無可用，則使用帳戶中的所有聯繫人。
   >
   >**隱式**:所有聯繫人（無論角色如何）。

>[!CAUTION]
>
>使用時 **隱式**,Marketo一律會檢查與帳戶相關聯的所有聯絡人（無論角色為何）。 **Marketo強烈建議使用明確模式**. 使用隱式可能會產生誤判；即，儘管對機會沒有實際影響力，但對機會有信譽的人。 請謹慎使用隱式。
