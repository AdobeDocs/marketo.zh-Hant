---
unique-page-id: 1146901
description: 使用進階智慧清單規則邏輯 — Marketo檔案 — 產品檔案
title: 使用高級智慧清單規則邏輯
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 使用高級智慧清單規則邏輯 {#using-advanced-smart-list-rule-logic}

將智慧清單規則邏輯套用至智慧清單內的多個篩選器，即可找到您需要的確切人員。 這是方法。

>[!PREREQUISITES]
>
>* [尋找篩選器並新增至智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [定義智慧清單篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>進階篩選邏輯僅在智慧清單中有三個或三個以上篩選器時才可用。

## 將邏輯添加到智慧清單 {#add-logic-to-a-smart-list}

預設情況下，智慧清單將查找匹配的人員 **全部** 篩選器（篩選器） _和_ 2 _和_ 3)。 您可以變更規則邏輯以尋找符合的人 **任何** （篩選器1） _或_ 2 _或_ 3)，或使用進階篩選(篩選器1 _和_ 2 _或_ 3)。

在此範例中，假設您想在加州尋找人員 _和_ 得分至少50分 _或_ 狀態為「合格銷售」。

1. 選擇 **使用進階篩選** 從下拉式清單中。

   ![](assets/one.png)

   >[!NOTE]
   >
   >使用 **進階** 篩選器減少了使用智慧清單成員篩選器建立智慧清單的需要。 這有助於最佳化效能。

1. 此 **進階篩選** 文字方塊會在所有篩選器之間顯示「和」作為預設值。

   ![](assets/two-2.png)

1. 在「2」和「3」之間鍵入一對括弧。

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >輸入規則邏輯時，您必須在「或」之前使用「和」。

1. 將「2」與「3」之間的「和」變更為「or」。

   ![](assets/four-1.png)

## 混合&quot;And&quot;和&quot;Or時使用括弧 {#use-parentheses-when-mixing-and-and-or}

混合&quot;and&quot;和&quot;or&quot;邏輯需要括弧來清楚說明您的意圖。

![](assets/advancedfilters-parent.png)

## 視需要為四個或更多個篩選器使用巢狀括弧 {#use-nested-parentheses-for-four-or-more-filters-if-needed}

根據您的意圖，使用四個或多個篩選器時，您可能需要新增巢狀括弧。

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>如果輸入無效規則，規則下會顯示紅線。 捲動到文字上以查看相關錯誤訊息。
