---
unique-page-id: 2949413
description: 為智慧清單篩選器新增限制 — Marketo檔案 — 產品檔案
title: 向智慧清單篩選器添加約束
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# 向智慧清單篩選器添加約束 {#add-a-constraint-to-a-smart-list-filter}

建立智慧清單時，有些篩選器有名為「限制」的進階選項。 這些是額外的條件，您可以新增至篩選器和觸發器，進一步縮小搜尋範圍。

在此範例中，將一些限制新增至 **[資料值已變更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** 篩選器，查找狀態從MQL更改為SQL的人員。

>[!PREREQUISITES]
>
>* [建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [在智慧清單中使用「資料值已變更」篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)
>


1. 前往 **行銷活動**.

   ![](assets/ma-1.png)

1. 選擇智慧清單，該清單包含要添加約束的篩選器，然後按一下 **智慧清單** 標籤。

   ![](assets/two-3.png)

1. 在 **添加約束**，選取 **上一個值**.

   ![](assets/three-3.png)

1. 輸入 **上一個值**. 在此示例中，我們使用MQL。

   ![](assets/four-2.png)

1. 在 **添加約束**，選取 **新值**.

   ![](assets/five.png)

1. 輸入 **新值**. 在此示例中，我們使用SQL。

   ![](assets/six.png)

1. 幹得好！ 按一下 **人員** 頁簽，查看 **狀態** 變更 **MQL** to **SQL** 過去30天。
