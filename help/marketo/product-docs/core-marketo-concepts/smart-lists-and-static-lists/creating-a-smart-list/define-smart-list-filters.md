---
unique-page-id: 557316
description: 定義智慧清單篩選器 — Marketo檔案 — 產品檔案
title: 定義智慧清單篩選器
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# 定義智慧清單篩選器 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [尋找並新增篩選器至智慧列示](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

現在您已[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}並在其中新增[篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}，接下來讓我們定義篩選器。 方法如下。

繼續我們的範例，讓我們定義這些篩選器，以尋找在加州分數超過50的所有人。

1. 移至&#x200B;**[!UICONTROL 行銷活動]**。

   ![](assets/define-smart-list-filters-1.png)

1. 選取想要的智慧列示，然後按一下&#x200B;**[!UICONTROL 智慧列示]**&#x200B;索引標籤。

   ![](assets/define-smart-list-filters-2.png)

1. 尋找並選取&#x200B;**[!UICONTROL 狀態]**&#x200B;篩選器的[CA]。

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >您可能會同時儲存「加州」和「CA」。 若要篩選這兩個值並包含來自加州的&#x200B;_所有_&#x200B;人員，瞭解如何[將多個值新增至智慧清單篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}。

1. 選取&#x200B;**[!UICONTROL 大於]**&#x200B;運運算元並輸入「50」。

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>如果您認為資料庫中可能有一些記錄包含不完整的電子郵件地址(例如，只有「@adobe.com」)，請在使用「contains」運運算元時使用兩個電子郵件地址篩選器。 一個含有「包含@adobe.com」的篩選器，以及一個含有「包含adobe.com」的個別篩選器（省略@符號）。

現在您知道如何建立智慧列示，以及新增/定義篩選器。
