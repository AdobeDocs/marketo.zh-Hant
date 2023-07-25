---
unique-page-id: 557316
description: 定義智慧清單篩選器 — Marketo檔案 — 產品檔案
title: 定義智慧清單篩選器
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 定義智慧清單篩選器 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [建立智慧清單](create-a-smart-list.md)
>* [尋找並新增篩選器至智慧清單](find-and-add-filters-to-a-smart-list.md)

現在您已完成 [已建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 和 [已新增篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) 開始使用時，讓我們定義篩選器。 方法如下。

繼續我們的範例，讓我們定義這些篩選器，以尋找評分超過50分的所有加州人。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-1.png)

1. 選取智慧清單，然後按一下 **智慧清單** 標籤。

   ![](assets/smarlist-choosefilters.png)

1. 尋找並選取 **CA** 的 **州** 篩選。

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >您可能正在儲存兩者 **加州** 和 **CA**. 為了篩選這兩個值和包含 _全部_ 加州人，瞭解如何  [新增多個值至智慧清單篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. 選取 **大於** 運運算元並輸入 **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>如果您認為資料庫中可能有一些記錄包含不完整的電子郵件地址(例如，只有「@adobe.com」)，請使用 **二** 使用「包含」運運算元時的電子郵件地址篩選器。 一個篩選器有「包含@adobe.com」，另一個篩選器有「包含adobe.com」（不含@符號）。

您現在知道如何建立智慧清單及新增/定義篩選器。
