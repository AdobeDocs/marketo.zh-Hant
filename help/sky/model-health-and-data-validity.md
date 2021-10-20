---
title: 模型健康與資料有效性
description: 模型健康與資料有效性
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
source-git-commit: 42ddb44100a041a09ff4a68c02ccf6aabb2d953e
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 模型健康與資料有效性

模型的效能取決於輸入資料的品質和完整性。 查看每個可能性AI模型的最大影響因素。 另請見導致事件註冊次數增加/減少、事件出席率或取消訂閱率的上層因素。

>[!NOTE]
>
>標示為(+)的行為對預測有正面影響（反之亦然）。

下面是如何評估模型健康度。

導覽至 **[!UICONTROL Models and Data Health]** 一節 **[!UICONTROL Predictive Audiences]** 在 **[!UICONTROL Admin]** Marketo Classic地區。 在此，您會看到所有模型及其狀態。

![影像一](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **培訓狀態**:指出您的模型是否在主動訓練（改善預測）。 每2週自動進行一次培訓。 任何 _處理_ 可能需要24小時才能完成。 適用於任何 _失敗_ 型號，請聯繫 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support).
* **計分狀態**:指出您的模型是否主動計算方案成員的預測（可能性百分比）。
* **效能**：根據資料完整性和資料品質來分類模型健全狀態（請參閱下方）。
* **資料完整性**:存在/完成的資料屬性百分比。
* **資料品質**:包含良好、可用資料的屬性百分比。
