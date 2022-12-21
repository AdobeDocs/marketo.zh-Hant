---
unique-page-id: 2953132
description: 了解批次和觸發智慧型行銷活動 — Marketo檔案 — 產品檔案
title: 了解批次和觸發智慧型促銷活動
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 了解批次和觸發智慧型促銷活動 {#understanding-batch-and-trigger-smart-campaigns}

智慧型行銷活動有兩種類型：批次和觸發。

## 批次智慧型促銷活動 {#batch-smart-campaign}

>[!NOTE]
>
>**定義**
>
>批次促銷活動會在特定時間啟動，並同時影響特定的一組人員。 例如，會傳送電子郵件給加州的所有人。

批次智慧型促銷活動在智慧型清單區段內只會有篩選器（亦即沒有觸發器）。

![](assets/batch-filter.png)

按一下 **排程** 標籤會確認智慧型促銷活動已設為「批次」。

![](assets/batch-c4.png)

**批次智慧型促銷活動**

* 可排程重複執行，例如每日、每週和每月。 你也可以讓他們只執行一次。
* 在 [方案排程檢視](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). 智慧型促銷活動中「等待」步驟之後的任何項目都不會包含在檢視中。

<br> 

## 觸發智慧型行銷活動 {#trigger-smart-campaign}

>[!NOTE]
>
>**定義**
>
>觸發智慧型促銷活動會根據觸發事件一次影響一個人。 觸發器的範例會是按一下電子郵件中的連結。

如果智慧型促銷活動在智慧型清單區段內使用至少一個觸發器，則模式會自動設為觸發。

![](assets/trigger.png)

按一下 **排程** 標籤會確認智慧型促銷活動已設為「已觸發」。

![](assets/trigger2.png)

**觸發智慧型行銷活動**

* 無法為重複計畫。 它們只能設為使用中或非使用中。
* 您可以設定多個觸發器。 不過，如果觸發了任何觸發器，則會執行促銷活動動作。

>[!TIP]
>
>使用 [活動記錄](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) 來查看智慧型行銷活動中的逐步發生項目。 您可以在人員詳細資訊頁面的最後一個索引標籤中找到活動記錄。
