---
unique-page-id: 2360217
description: 變更Analytics的歸因設定 — Marketo檔案 — 產品檔案
title: 變更Analytics歸因設定
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# 變更Analytics歸因設定 {#change-attribution-settings-for-analytics}

您可以變更Marketo將聯絡人與首次接觸與多次接觸歸因的機會、潛在客戶轉換量度及行銷影響的機會標幟連結的方式。

這些設定將影響[方案機會分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)、[機會分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)和潛在客戶分析區域下的[!UICONTROL 收入總管]報告。 這也會影響[!UICONTROL 程式分析器]報告。

1. 移至&#x200B;**[!UICONTROL 管理員]**&#x200B;區域。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 按一下&#x200B;**[!UICONTROL 收入週期分析]**。

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 按一下&#x200B;**[!UICONTROL 歸因]**&#x200B;下的&#x200B;**[!UICONTROL 編輯]**&#x200B;連結。

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >變更此設定不會修改任何Marketo資料；只會變更報表的執行方式。 這可以隨時還原。

1. 選取選項並按一下&#x200B;**[!UICONTROL 儲存]**。

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**[!UICONTROL 明確]**：僅具有角色的連絡人（預設）。
   >
   >**[!UICONTROL 混合式]**：具有角色的連絡人（如果有的話）。 如果沒有可用專案，則會使用帳戶中的所有連絡人。
   >
   >**[!UICONTROL 隱含]**：所有連絡人，不論角色為何。

>[!CAUTION]
>
>使用&#x200B;**[!UICONTROL Implicit]**&#x200B;時，無論角色為何，Marketo一律會檢查與該帳戶相關聯的所有連絡人。 **Marketo強烈建議使用[!UICONTROL 明確]模式**。 使用[!UICONTROL 隱含]可能會產生誤判；也就是說，雖然對商機沒有實際影響，但擁有商機評分的人員。 請謹慎使用[!UICONTROL 隱含]。
