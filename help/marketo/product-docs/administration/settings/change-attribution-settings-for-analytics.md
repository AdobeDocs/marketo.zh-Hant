---
unique-page-id: 2360217
description: 變更Analytics的歸因設定 — Marketo檔案 — 產品檔案
title: 變更Analytics歸因設定
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# 變更Analytics歸因設定 {#change-attribution-settings-for-analytics}

您可以變更Marketo將聯絡人與商機連結的方式，以取得首次接觸和多點接觸歸因、潛在客戶轉換量度，以及受行銷影響的商機標幟。

這些設定將影響 [!UICONTROL 收入總管] 下的報表 [計畫機會分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)， [機會分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)和銷售機會分析區域。 這也會影響 [!UICONTROL 程式分析器] 報告。

1. 前往 **[!UICONTROL 管理員]** 區域。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 按一下 **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 按一下 **[!UICONTROL 編輯]** 連結於 **[!UICONTROL 歸因]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >變更此設定不會修改任何Marketo資料，只會變更報表的執行方式。 這可以隨時還原。

1. 選取選項並按一下 **[!UICONTROL 儲存]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**[!UICONTROL 明確]**：僅具有角色的聯絡人（預設）。
   >
   >**[!UICONTROL 混合式]**：具有角色的聯絡人（若有）。 如果沒有可用專案，則會使用帳戶中的所有連絡人。
   >
   >**[!UICONTROL 隱含]**：所有連絡人，不論角色為何。

>[!CAUTION]
>
>使用時 **[!UICONTROL 隱含]**，無論角色為何，Marketo一律會檢查與帳戶相關聯的所有連絡人。 **Marketo強烈建議使用 [!UICONTROL 明確] 模式**. 使用 [!UICONTROL 隱含] 可能會產生誤判；例如，雖然對機會沒有實際影響，但擁有機會評分的人。 使用 [!UICONTROL 隱含] 請小心。
