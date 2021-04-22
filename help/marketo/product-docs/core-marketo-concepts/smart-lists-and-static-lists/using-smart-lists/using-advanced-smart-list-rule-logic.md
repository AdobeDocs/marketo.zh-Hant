---
unique-page-id: 1146901
description: 使用高級智慧清單規則邏輯-Marketo文檔——產品文檔
title: 使用高級智慧清單規則邏輯
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 使用高級智慧清單規則邏輯{#using-advanced-smart-list-rule-logic}

您可以將智慧型清單規則邏輯套用至智慧型清單中的多個篩選器，以找到所需的確切人員。 這是方法。

>[!PREREQUISITES]
>
>* [尋找並新增篩選器至智慧型清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [定義智慧清單篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>進階篩選邏輯僅在智慧型清單中有三個或三個以上的篩選器時可用。

## 將邏輯添加到智慧清單{#add-logic-to-a-smart-list}

根據預設，您的智慧型清單會找到符合&#x200B;**ALL**&#x200B;濾鏡（濾鏡1 _和_ 2 _和_ 3）的人員。 您可以變更規則邏輯，以尋找符合已定義篩選器（篩選器1 _或_ 2 _或_ 3）的&#x200B;**ANY**&#x200B;的人，或使用進階篩選器（篩選器1 _和_ 2 _或_ 3）。

在此範例中，假設您想要在加州找到&#x200B;_和_，分數至少為50分&#x200B;_或_&#x200B;且狀態為「銷售合格」的人。

1. 從下拉式清單中選取「使用進階篩選器&#x200B;**」。**

   ![](assets/one.png)

   >[!NOTE]
   >
   >使用&#x200B;**Advanced**&#x200B;篩選器可減少使用智慧清單成員篩選器建立智慧清單的需要。 這有助於優化效能。

1. **進階篩選器**&#x200B;文字方塊會顯示&quot;and&quot;，作為所有篩選器之間的預設值。

   ![](assets/two-2.png)

1. 在&quot;2&quot;和&quot;3&quot;周圍鍵入一對括弧。

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >在輸入規則邏輯時，您必須在「或」之前使用「and」。

1. 將&quot;2與3&quot;之間的&quot;and&quot;變更為&quot;or&quot;。

   ![](assets/four-1.png)

## 混合&quot;And&quot;和&quot;Or {#use-parentheses-when-mixing-and-and-or}時使用括弧

混合&quot;and&quot;和&quot;or&quot;邏輯需要括弧來清楚說明您的意圖。

![](assets/advancedfilters-parent.png)

## 如果需要{#use-nested-parentheses-for-four-or-more-filters-if-needed}，請對四個或更多篩選器使用巢狀括弧

視您的意圖而定，在使用四個或多個篩選器時，您可能需要新增巢狀括弧。

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>如果您輸入無效的規則，您會看到規則下方顯示紅線。 捲動至文字上，以檢視相關的錯誤訊息。
