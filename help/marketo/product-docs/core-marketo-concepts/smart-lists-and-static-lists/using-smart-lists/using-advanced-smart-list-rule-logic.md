---
unique-page-id: 1146901
description: 使用進階智慧清單規則邏輯 — Marketo檔案 — 產品檔案
title: 使用進階智慧列示規則邏輯
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 使用進階智慧列示規則邏輯 {#using-advanced-smart-list-rule-logic}

您可以將智慧清單規則邏輯套用至智慧清單中的多個篩選器，以找到所需的確切人員。 方法如下。

>[!PREREQUISITES]
>
>* [尋找篩選器並將其新增至智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [定義智慧清單篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>[!NOTE]
>
>進階篩選器邏輯僅適用於智慧清單中有三個或更多篩選器的情況。

## 將邏輯新增至智慧清單 {#add-logic-to-a-smart-list}

根據預設，您的智慧清單會尋找相符的人員 **全部** 篩選器（篩選器1） _和_ 2 _和_ 3)。 您可以變更規則邏輯，以尋找相符的人員 **任何** 已定義的篩選器（篩選器1） _或_ 2 _或_ 3)，或使用進階篩選器(篩選器1 _和_ 2 _或_ 3)。

在此範例中，假設您想尋找加州的人 _和_ 分數至少為50分 _或_ 狀態為「銷售合格」。

1. 選取 **使用進階篩選** 下拉式清單。

   ![](assets/one.png)

   >[!NOTE]
   >
   >使用 **進階** 濾鏡可減少使用「智慧列示成員」濾鏡建立智慧列示的需求。 這有助於最佳化效能。

1. 此 **進階篩選** 文字方塊會顯示「和」作為所有篩選器之間的預設值。

   ![](assets/two-2.png)

1. 在「2和3」周圍鍵入一對括弧。

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >輸入規則邏輯時，您必須在「或」之前使用「and」。

1. 將「2 and 3」之間的「and」變更為「or」。

   ![](assets/four-1.png)

## 混合「And」和「Or」時使用括弧 {#use-parentheses-when-mixing-and-and-or}

混合「and」和「or」邏輯需要括弧來清楚表示您的意圖。

![](assets/advancedfilters-parent.png)

## 視需要使用巢狀括弧括住四個或更多篩選器 {#use-nested-parentheses-for-four-or-more-filters-if-needed}

根據您的意圖，在使用四個或更多篩選器時，您可能需要新增巢狀括弧。

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>如果輸入無效的規則，您會在規則下方看到一條紅線。 捲動文字以檢視相關的錯誤訊息。
