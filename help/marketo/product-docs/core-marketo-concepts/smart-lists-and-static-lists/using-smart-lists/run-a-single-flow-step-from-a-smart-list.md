---
unique-page-id: 557322
description: 從智慧清單執行單一流程步驟 — Marketo檔案 — 產品檔案
title: 從智慧清單執行單一流程步驟
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# 從智慧清單執行單一流程步驟 {#run-a-single-flow-step-from-a-smart-list}

如果您想執行僅一次的流量步驟，則可在智慧清單內使用單一流量步驟，而非建立整個智慧促銷活動。

>[!PREREQUISITES]
>
>[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-1.png)

1. 選擇包含人員的清單或智慧清單，然後轉至 **人員** 標籤。

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >靜態清單和智慧清單都具有此功能。

1. 按一下 **全選**. 您也可以使用 **Ctrl/Cmd** 然後按一下，手動選擇一些記錄。

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >如果結果跨越多個頁面，請按一下 **全選** 會選取所有頁面上的所有人員。

1. 在 **人員** **動作**，請選取您選取的流程步驟。 在此範例中，我們將使用 [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. 尋找並選取 **屬性**. 在此範例中，我們會將所有擁有「加州」的人，變更為「CA」。

   ![](assets/runaction-hands.png)

1. 輸入新值. 按一下 **立即運行**.

   ![](assets/runactionnewvalue-hands.png)

1. 如果您要變更大量人員的資料值，可能需要輸入數字以確認變更。 按一下 **Go It**.

   ![](assets/changedatavalue.jpg)

太棒了！ 您會在右上角看到單一流量步驟的狀態。

![](assets/completesingleflowaction.jpg)

完成後，重新整理清單，您就會看到更新的資訊。
