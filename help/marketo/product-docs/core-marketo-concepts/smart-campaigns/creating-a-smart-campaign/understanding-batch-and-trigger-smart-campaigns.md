---
unique-page-id: 2953132
description: 瞭解批次和觸發智慧行銷活動 — Marketo檔案 — 產品檔案
title: 瞭解批次和觸發智慧行銷活動
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 瞭解批次和觸發智慧行銷活動 {#understanding-batch-and-trigger-smart-campaigns}

智慧行銷活動有兩種型別：批次和觸發。

## 批次Smart Campaign {#batch-smart-campaign}

>[!NOTE]
>
>**定義**
>
>批次行銷活動會在特定時間啟動，並一次影響一組特定人員。 例如，傳送電子郵件給加州的所有人。

批次智慧行銷活動將只有智慧清單區段中的篩選器（即沒有觸發器）。

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

按一下 **排程** 索引標籤會確認智慧型行銷活動已設為「批次」。

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**批次智慧型行銷活動**

* 可以排程為遞回，例如每日、每週和每月。 您也可以讓這些變數執行一次。
* 顯示在 [方案排程檢視](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). 在Smart Campaign中「等待」步驟之後的任何專案都不會包含在檢視中。

<br> 

## 觸發Smart Campaign {#trigger-smart-campaign}

>[!NOTE]
>
>**定義**
>
>觸發智慧行銷活動會根據觸發的事件，一次影響一個人。 觸發器的範例為按一下電子郵件中的連結。

如果智慧行銷活動在智慧列示區段內使用至少一個觸發器，模式會自動設定為觸發。

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

按一下 **排程** 索引標籤會確認智慧型行銷活動已設為「已觸發」。

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**觸發智慧行銷活動**

* 無法排程遞回。 它們只能設定為作用中或非作用中。
* 您可以設定多個觸發器。 不過，如果觸發了任何觸發器，就會執行行銷活動動作。

>[!TIP]
>
>使用 [活動記錄](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) 檢視在您的Smart Campaigns中逐步發生的事情。 您可以在人員詳細資訊頁面的最後一個標籤中找到活動記錄。
