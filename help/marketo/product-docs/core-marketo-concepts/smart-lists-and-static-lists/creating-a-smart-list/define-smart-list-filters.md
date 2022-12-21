---
unique-page-id: 557316
description: 定義智慧清單篩選器 — Marketo檔案 — 產品檔案
title: 定義智慧清單篩選器
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 定義智慧清單篩選器 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [建立智慧清單](create-a-smart-list.md)
>* [尋找篩選器並新增至智慧清單](find-and-add-filters-to-a-smart-list.md)


既然你 [建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 和 [新增篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) 我們來定義篩選器。 這是方法。

繼續我們的範例，讓我們定義這些篩選器，以尋找在加州分數超過50的所有人。

1. 前往 **行銷活動**.

   ![](assets/login-marketing-activities-1.png)

1. 選取智慧清單，然後按一下 **智慧清單** 標籤。

   ![](assets/smarlist-choosefilters.png)

1. 查找和選擇 **CA** 針對 **狀態** 篩選。

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >你可能同時儲存 **加州** 和 **CA**. 若要同時篩選這兩個值，請納入 _all_ 加州人，學習如何  [將多個值添加到智慧清單篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. 選擇 **大於** 運算子和輸入 **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>如果您認為資料庫中可能有某些記錄包含不完整的電子郵件地址(例如，只有&quot;@adobe.com&quot;)，請使用 **two** 使用「包含」運算子時的電子郵件地址篩選。 一個篩選器包含「contains @adobe.com」，另一個篩選器包含「contains adobe.com」（遺漏@符號）。

您現在知道如何建立智慧清單及新增/定義篩選器。
