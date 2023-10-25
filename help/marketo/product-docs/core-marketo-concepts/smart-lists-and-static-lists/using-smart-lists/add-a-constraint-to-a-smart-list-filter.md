---
unique-page-id: 2949413
description: 新增限制至智慧清單篩選器 — Marketo檔案 — 產品檔案
title: 新增限制至智慧清單篩選器
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: aeefe7a5c265e3a7ddd50920820742a463ab178a
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# 新增限制至智慧清單篩選器 {#add-a-constraint-to-a-smart-list-filter}

建立智慧列示時，有些篩選器會具有稱為「限制」的進階選項。 這些是可新增至篩選器和觸發器的額外條件，有助於進一步縮小搜尋範圍。

在此範例中，我們將一些限制新增至 **[資料值已變更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** 篩選以尋找狀態從MQL變更為SQL的人員。

>[!PREREQUISITES]
>
>* [建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [在智慧清單中使用「資料值已變更」篩選器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. 前往 **[!UICONTROL 行銷活動]**.

   ![](assets/ma-1.png)

1. 選取含有您即將新增限制的篩選器的智慧清單，然後按一下 **[!UICONTROL 智慧清單]** 標籤。

   ![](assets/two-3.png)

1. 在 **[!UICONTROL 新增限制]**，選取 **[!UICONTROL 上一個值]**.

   ![](assets/three-3.png)

1. 輸入 **[!UICONTROL 上一個值]**. 在此範例中，我們使用MQL。

   ![](assets/four-2.png)

1. 在 **[!UICONTROL 新增限制]**，選取 **[!UICONTROL 新值]**.

   ![](assets/five.png)

1. 輸入新值。 在此範例中，我們使用SQL。

   ![](assets/six.png)

1. 做得很好！ 按一下 **[!UICONTROL 人員]** tab來檢視在過去30天內具有Status從「MQL」變更為「SQL」的所有人員。
