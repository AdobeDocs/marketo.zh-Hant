---
unique-page-id: 4718683
description: 核准階段並將潛在客戶指派至收入模型 — Marketo檔案 — 產品檔案
title: 核准階段並指派銷售機會至收入模型
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 核准階段並指派銷售機會至收入模型 {#approving-stages-and-assigning-leads-to-a-revenue-model}

取得您的 **收入模型** 新增現有銷售機會，並為任何新銷售機會建立指派規則，以啟動並執行。

## 核准階段 {#approving-stages}

新增任何潛在客戶之前，請先核准模型的各個階段。

1. 前往 **分析** 區域。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 選取您要核准其階段的模型。

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. 下 **模型動作**，選取 **核准階段**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. 系統會以警示迎接您；按一下 **指派銷售機會**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

太棒了！ 讓我們繼續並指派這些銷售機會。

## 指派現有銷售機會 {#assigning-existing-leads}

[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 識別Lead資料庫中模型某一階段的潛在客戶。

1. 一旦您擁有 [已建立您的智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)，按一下 **銷售機會** 標籤。

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. 按一下 **全選** 以選取銷售機會。

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. 開啟 **潛在客戶動作** 下拉式清單並選取 **特殊**. 按一下 **變更收入階段**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. 選取正確的 **模型** 和正確的 **階段**. 按一下 **立即執行**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. 重複此步驟，直到所有潛在客戶都已指派至模型的各個階段為止。

太棒了！ 若要指定將新潛在客戶指派給階段的方式，請建立指派規則。

>[!NOTE]
>
>如果您的模型處於「已核准階段」狀態，則潛在客戶活動記錄中不會顯示任何「變更收入階段」事件。 如果您的模型已完全核准，如果您將潛在客戶移動到其目前所在的相同階段，則會跳過此流程步驟。

## 新銷售機會：建立指定規則  {#new-leads-create-assignment-rules}

1. 按一下 **Marketo首頁** 再次，然後選取 **分析**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 在樹狀結構中按一下您的模型，然後 **模型動作** 功能表，選取 **指派規則**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. 如果您的指派規則包含多個預設選擇，請按一下 **階段**，進行選取，然後按一下 **新增選擇**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## 指派規則範例 {#example-assignment-rule}

建立「銷售機會分數」規則，以將具有最低分數的新銷售機會指派給適當的步驟。

1. 下 **若**，選取 **潛在客戶分數**. 然後選擇 **至少**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. 輸入 **40** 在欄位中並選取 **銷售機會** 作為階段。 按一下 **儲存** 完成。

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>若要核准您的模型，請閱讀我們的說明頁面： **[核准和取消核准收入模型](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
