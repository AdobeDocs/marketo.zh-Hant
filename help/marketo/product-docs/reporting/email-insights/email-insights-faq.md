---
unique-page-id: 10100257
description: 電子郵件深入分析常見問題集 — Marketo檔案 — 產品檔案
title: 電子郵件深入分析常見問題集
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 電子郵件深入分析常見問題集 {#email-insights-faq}

## 「電子郵件分析」的比率量度與其他Marketo電子郵件報告之間是否有任何差異？ {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

是. 電子郵件深入分析針對計算參與量度比率（開啟率、點按開啟率、取消訂閱率）時傳送的相同電子郵件，將參與量度與其對應的傳送量度建立關聯。 例如，在電子郵件深入分析中，檢視過去一週包含每日點按開啟率劃分的時間序列圖表時，我們現在會根據對應的傳送量度，顯示開啟/點按/取消訂閱事件的真正相關比率。 這與Revenue Explorer中的行為形成對照，後者只是一切的總和。 電子郵件深入分析可更準確地檢視參與率。

## 為什麼電子郵件深入分析僅支援10個自訂Dimension？ {#why-does-email-insights-only-support-custom-dimensions}

對於許多使用案例，以10個額外的自訂維度擴充預設系統維度已足夠，並包括根據分段或計畫標籤的自訂維度。 我們計畫在未來允許客戶增加允許的自訂Dimension數量。

## 為何無法在指派後重複使用自訂Dimension槽？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

分配指定的「自訂Dimension」位置後，重新對應它會導致先前的資料在與新含義混合時產生錯誤。 因此，自訂Dimension位置可能無法重複使用。 此行為與其他量度分析工具(例如Google Analytics)的行為一致。

## 電子郵件深入分析是否支援Marketo銷售深入分析電子郵件？ {#does-email-insights-support-marketo-sales-insight-emails}

是. 所有透過Marketo Sales Insights傳送的電子郵件都會包含在電子郵件深入分析中。

## 電子郵件深入分析是否支援營運電子郵件？ {#does-email-insights-support-operational-emails}

是. 依預設，檢視和查詢會隱藏營運電子郵件。 不過，您可以在「個人設定」面板下變更此設定。

## 電子郵件深入分析是否會擷取週期性排程或重新執行Smart Campaign電子郵件流程步驟？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

「是」與「否」。 在電子郵件深入分析的初始版本中，所有電子郵件事件皆會被擷取，並可供任何循環排程或重新執行的Smart Campaign存取。 但您無法區分該Smart Campaign的不同執行。 我們將在下一個版本中新增支援，以擷取「開啟」、「點按」和「取消訂閱」事件的Smart Campaign執行資訊，進而加以區分。

## 依裝置型別或裝置作業系統篩選時，為何許多量度會顯示零？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除了點按開啟率、開啟、點按和取消訂閱之外，所有其他支援的量度都是傳遞事件或衍生自傳遞事件的比率。 由於裝置型別和裝置作業系統僅適用於參與量度，因此我們完全沒有資訊可顯示。 例如，在依裝置型別=行動裝置篩選時詢問傳遞率是未定義的查詢，因為Marketo可能沒有收到基礎傳遞和已傳送事件的任何參與量度。 我們正在探索如何從參與量度套用裝置型別和裝置作業系統，以取得包含參與和傳送量度的比率。

## 當某些電子郵件使用者端封鎖影像時，「電子郵件深入分析」會做什麼？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

一個常見的產業問題是越來越多的電子郵件使用者端預設會關閉影像。 載入影像是記錄「開啟」的基礎。 使用者完全有可能收到含有已封鎖影像的電子郵件，但文字和連結完全可讀。 如果使用者遇到這個情況，並按一下該電子郵件中的連結，您最後會遇到點按事件的情況，但不會收到該電子郵件對應的「開啟」事件。 Marketo電子郵件深入分析會自動產生任何遺失的事件。 邏輯與Marketo對電子郵件效能報表以及Revenue Explorer中的電子郵件分析區域執行的操作相同。
