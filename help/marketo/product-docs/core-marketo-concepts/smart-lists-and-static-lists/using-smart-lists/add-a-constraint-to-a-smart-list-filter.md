---
unique-page-id: 2949413
description: 新增限制至智慧型清單篩選——行銷人員檔案——產品檔案
title: 將約束添加到智慧清單過濾器
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# 將約束添加到智慧清單過濾器 {#add-a-constraint-to-a-smart-list-filter}

在建立智慧型清單時，有些篩選器有稱為*constraints的進階選項。 *您可以將這些額外條件新增至篩選器和觸發器，以進一步縮小搜尋範圍。

在此示例中，讓我們將一些約束添加到** [Data Value Changed](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**篩選器中，以查找狀態從MQL更改為SQL的人員。

>[!PREREQUISITES]
>
>* [建立智慧清單](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [在智慧型清單中使用「資料值變更」篩選](use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. 前往行 **銷活動**。

   ![](assets/ma-1.png)

1. 選擇智慧清單，其中包含要向其添加約束的過濾器，然後按一下「智慧列 **表」頁籤** 。

   ![](assets/two-3.png)

1. 在「添 **加約束**」(Add Constraint **)下，選**&#x200B;擇「上一值」(Previous Value)。

   ![](assets/three-3.png)

1. 輸入上 **一個值**。 在此示例中，我們使用MQL。

   ![](assets/four-2.png)

1. 在「添 **加約束**」(Add Constraint)下，選 **擇「新值」(New Value**)。

   ![](assets/five.png)

1. 輸入 **新值**。 在此示例中，我們使用SQL。

   ![](assets/six.png)

1. 幹得漂亮！ 按一下「 **People** 」頁籤可查看在過去30天內狀態從 **MQL** 變更為 ******** SQL Changed的所有人員。

