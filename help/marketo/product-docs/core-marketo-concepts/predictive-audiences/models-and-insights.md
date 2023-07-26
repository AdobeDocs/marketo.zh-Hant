---
description: 模型與深入分析 — Marketo檔案 — 產品檔案
title: 模型與深入分析
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# 模型與深入分析 {#models-and-insights}

模型的效能取決於輸入資料的品質和完整性。 檢視每個可能性AI模型的最大影響因素。 另請參閱造成高/低事件註冊、事件出席或取消訂閱次數的主要因素。

>[!NOTE]
>
>以(+)標籤的行為會對預測產生正面影響（反之亦然）。

以下說明如何評估您的模型健康情況。

導覽至 **[!UICONTROL 模型與資料健康狀態]** 區段在 **[!UICONTROL 預測對象]** 在 **[!UICONTROL 管理員]** Marketo Engage區域。 您將在這裡看到您的所有模型及其狀態。

![影像1](assets/models-and-insights-1.png)

* **訓練狀態**：指出模型是否正在積極訓練（改善預測）。 每2週自動進行訓練。 任何符合下列條件的模型： _處理中_ 最多可能需要24小時的時間才能完成。 針對任何 _已失敗_ 型號，請聯絡 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.
* **評分狀態**：指出您的模型是否正在主動計算方案成員的預測（可能性百分比）。
* **效能**：根據資料完整性和資料品質將您的模型健康情況分類（請參閱下文）。
* **資料完整性**：出現/完成的資料屬性百分比。
* **資料品質**：包含良好、可用資料的屬性百分比。
