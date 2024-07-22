---
unique-page-id: 4718683
description: 核准階段並指派銷售機會至收入模型 — Marketo檔案 — 產品檔案
title: 核准階段並將銷售機會指定至收入模型
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# 核准階段並將銷售機會指定至收入模型 {#approving-stages-and-assigning-leads-to-a-revenue-model}

新增現有的銷售機會，並為任何新的銷售機會建立指派規則，以啟動並執行您的&#x200B;**收入模型**。

## 核准階段 {#approving-stages}

在新增任何潛在客戶之前，先讓我們核准您的模型的階段。

1. 移至&#x200B;**Analytics**&#x200B;區域。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 選取您要核准其階段的模型。

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. 在&#x200B;**模型動作**&#x200B;下，選取&#x200B;**核准階段**。

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. 系統會以警示迎接您；按一下&#x200B;**指派銷售機會**。

   ![](assets/image2015-4-28-17-3a5-3a39.png)

太好了！ 讓我們繼續並指派這些銷售機會。

## 指派現有銷售機會 {#assigning-existing-leads}

[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)，以識別潛在客戶資料庫中模型某一階段的潛在客戶。

1. 在您[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)後，請按一下&#x200B;**銷售機會**&#x200B;標籤。

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. 按一下&#x200B;**全選**&#x200B;以選取銷售機會。

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. 開啟&#x200B;**潛在客戶動作**&#x200B;下拉式清單，並選取&#x200B;**特殊專案**。 按一下&#x200B;**變更收入階段**。

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. 選取正確的&#x200B;**模型**&#x200B;和正確的&#x200B;**階段**。 按一下&#x200B;**立即執行**。

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. 重複此步驟，直到您將所有銷售機會指派給模型的各個階段為止。

太棒了！ 若要指定將新潛在客戶指派給階段的方式，請建立指派規則。

>[!NOTE]
>
>如果您的模型處於「已核准階段」狀態，您將不會在潛在客戶的活動記錄中看到任何「變更收入階段」事件。 如果您的模型已完全核准，則如果您將銷售機會移至其目前所在的相同階段，將會略過此流程步驟。

## 新銷售機會：建立指定規則  {#new-leads-create-assignment-rules}

1. 再按一下&#x200B;**Marketo首頁**，然後選取&#x200B;**Analytics**。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 按一下樹狀結構中的模型，然後選取&#x200B;**模型動作**&#x200B;功能表，選取&#x200B;**指派規則**。

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. 如果您的指派規則包含多個預設選擇，請按一下&#x200B;**階段**，進行您的選擇，然後按一下&#x200B;**新增選擇**。

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## 指派規則範例 {#example-assignment-rule}

建立「銷售機會分數」規則，將分數最低的新銷售機會指派給適當的步驟。

1. 在&#x200B;**If**&#x200B;下，選取&#x200B;**潛在客戶分數**。 然後選擇&#x200B;**至少**。

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. 在欄位中輸入&#x200B;**40**，然後選取&#x200B;**銷售機會**&#x200B;作為階段。 按一下&#x200B;**儲存**&#x200B;以完成。

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>若要核准您的模型，請閱讀&#x200B;**[核准和取消核准收入模型](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**&#x200B;上的說明頁面。
