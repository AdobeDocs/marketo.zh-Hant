---
unique-page-id: 557316
description: 定義智慧清單篩選器 — Marketo文檔 — 產品文檔
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
>* [查找篩選器並將其添加到智慧清單](find-and-add-filters-to-a-smart-list.md)


既然你 [建立了智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 和 [添加的篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) 我們來定義過濾器。 這是方法。

繼續我們的示例，讓我們定義這些篩選器以查找在加利福尼亞得分超過50的所有人。

1. 轉到 **營銷活動**。

   ![](assets/login-marketing-activities-1.png)

1. 選擇智慧清單，然後按一下 **智慧清單** 頁籤。

   ![](assets/smarlist-choosefilters.png)

1. 查找並選擇 **CA** 為 **州** 的子菜單。

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >您可能正在儲存 **加利福尼亞** 和 **CA**。 為了篩選兩個值並包括 _全部_ 加州人，學著  [將多個值添加到智慧清單篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md)。

1. 選擇 **大於** 運算子和輸入 **50**。

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>如果您認為資料庫中可能包含不完整電子郵件地址(例如，僅&quot;@adobe.com&quot;)的一些記錄，請使用 **二** 使用「contains」運算子時，電子郵件地址篩選器。 一個包含「contains @adobe.com」的篩選器，另一個包含「contains adobe.com」的篩選器（省略@符號）。

您現在知道如何建立智慧清單和添加/定義篩選器。
