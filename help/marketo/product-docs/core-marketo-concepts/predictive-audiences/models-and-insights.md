---
description: 模型與深入分析 — Marketo檔案 — 產品檔案
title: 模型和洞察
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
source-git-commit: 8101d9c73571948847d00dfc21f21c39bcd1d975
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# 模型和洞察 {#models-and-insights}

模型的效能取決於輸入資料的品質和完整性。 檢視每個可能性AI模型的最大影響因素。 此外，也請檢視造成高/低事件註冊、事件出席率或取消訂閱的前幾個因素。

>[!NOTE]
>
>以(+)標籤的行為會對預測產生正面影響（反之亦然）。

以下說明如何評估您模型的健康情況。

導覽至Marketo Engage **[!UICONTROL Models and Data Health]**&#x200B;區域中&#x200B;**[!UICONTROL Predictive Audiences]**&#x200B;下的&#x200B;**[!UICONTROL Admin]**&#x200B;區段。 您將在這裡看到您的所有模型及其狀態。

![影像1](assets/models-and-insights-1.png)

* **訓練狀態**：指出您的模型是否正在主動訓練（改善預測）。 每兩週自動進行訓練。 任何&#x200B;_處理_&#x200B;的模型最多可能需要24小時才能完成。 對於任何&#x200B;_失敗_&#x200B;模型，請聯絡[Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}。
* **評分狀態**：指出您的模型是否正在主動計算方案成員的預測（可能性百分比）。
* **效能**：根據資料完整性和資料品質將模型狀況分類（請參閱下文）。
* **資料完整性**：存在/完成的資料屬性百分比。
* **資料品質**：包含良好可用資料的屬性百分比。
* **上次訓練時間**：目前模型與每兩週訓練的新模型之間評估中最佳的模型日期。
