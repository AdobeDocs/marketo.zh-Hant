---
description: 模型健康和資料有效性 — Marketo文檔 — 產品文檔
title: 模型健康與資料有效性
hide: true
hidefromtoc: true
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# 模型健康與資料有效性 {#model-health-and-data-validity}

模型的效能取決於輸入資料的質量和完整性。 查看每種可能性AI模型的最大影響因素。 另請參閱導致事件註冊、事件出席率或取消訂閱的最主要因素。

>[!NOTE]
>
>標籤為(+)的行為對預測產生積極影響（反之亦然）。

下面是如何評估您的模型健康狀況。

導航到 **[!UICONTROL 模型和資料運行狀況]** 節 **[!UICONTROL 預測受眾]** 的 **[!UICONTROL 管理]** Marketo Classic。 在此，您將看到所有模型及其狀態。

![影像1](assets/model-health-and-data-validity-1.png)

* **培訓狀態**:指示模型是否在積極培訓（改進預測）。 每兩週自動進行一次培訓。 任何 _處理_ 可能需要24小時才能完成。 對於任何 _失敗_ 型號，請聯繫 [Marketo支援](https://nation.marketo.com/t5/Support/ct-p/Support)。
* **計分狀態**:指示模型是否正在主動計算程式成員的預測（似然百分比）。
* **效能**：基於資料完整性和資料質量對模型運行狀況進行分類（請參閱下文）。
* **資料完整性**:存在/完成的資料屬性的百分比。
* **資料質量**:包含好可用資料的屬性的百分比。