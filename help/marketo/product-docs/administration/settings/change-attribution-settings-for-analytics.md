---
unique-page-id: 2360217
description: 變更Analytics的歸因設定——行銷人員檔案——產品檔案
title: 變更Analytics的歸因設定
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# 變更Analytics的歸因設定 {#change-attribution-settings-for-analytics}

您可以變更行銷人員將聯絡人與首次接觸和多次接觸歸因的商機、潛在客戶轉換度量，以及行銷影響的機會標幟的關聯方式。

這些設定將影響Program Opportunity Analysis [、](../../../product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)Opportunity Analysis [](../../../product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)和Lead Analysis區域下的Revenue Explorer報告。 這也會影響Program Analyzer報告。

1. 在「管理 **員** 」區段下，按一 **下「收入週期分析」**。

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. 按一下「 **歸因** 」下的「編 **輯」連結**。

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >變更此設定並不會修改任何Marketo資料；它只會改變報表的執行方式。 這可以隨時回復。

1. 選取選項，然後按一下「 **儲存**」。

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**定義**
   >
   >
   >**明確**:僅與角色聯繫（預設）。
   >
   >
   >**混合**:具有角色的聯繫人（如果可用）。 如果無可用，則會使用帳戶中的所有聯繫人。
   >
   >
   >**隱含**:所有聯繫人（不論角色）。

>[!CAUTION]
>
>使用隱 **含時**,Marketo一律會檢查與帳戶相關的所有連絡人，不論其角色為何。 **Marketo強烈建議使用顯式模式。** 使用隱式可能會造成誤報；即，儘管對機會沒有實際影響，但對機會有功勞的人。 謹慎使用隱含。

