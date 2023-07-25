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

是. 電子郵件深入分析針對計算參與量度比率（開啟率、點按開啟率、取消訂閱率）時傳送的相同電子郵件，將參與量度與其對應的傳送量度建立關聯。 例如，在電子郵件深入分析中，檢視過去一週的時間序列圖表（包含每日點按開啟率的劃分）時，我們現在會根據對應的傳送量度，顯示開啟/點按/取消訂閱事件的真正相關比率。 這與Revenue Explorer中的行為相反，後者只將所有內容加總。 電子郵件深入分析可更準確地檢視參與率。

## 為什麼Email Insights僅支援10個自訂Dimension？ {#why-does-email-insights-only-support-custom-dimensions}

對於許多使用案例，以10個額外的自訂維度擴充預設系統維度已足夠，並包括根據分段或計畫標籤的自訂維度。 未來，我們打算允許客戶增加允許的自訂Dimension數量。

## 為何無法在指派後重複使用自訂Dimension位置？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

分配指定的「自訂Dimension」位置後，重新對應會導致先前的資料在與新含義混合時產生錯誤。 因此，自訂Dimension位置可能無法重複使用。 此行為與其他量度分析工具(例如Google Analytics)的行為一致。

## 電子郵件深入分析是否支援Marketo Sales Insight電子郵件？ {#does-email-insights-support-marketo-sales-insight-emails}

是. 所有透過Marketo Sales Insights傳送的電子郵件都會包含在電子郵件分析中。

## 電子郵件深入分析是否支援營運電子郵件？ {#does-email-insights-support-operational-emails}

是. 依預設，在檢視和查詢中隱藏營運電子郵件。 不過，您可以在「個人設定」面板下變更此設定。

## 電子郵件分析會擷取週期性排程或重新執行Smart Campaign電子郵件流程步驟嗎？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

「是」與「否」。 透過Email Insights的初始版本，任何週期性排程或重新執行的Smart Campaign都能擷取及存取所有電子郵件事件。 但您無法區分該Smart Campaign的不同執行。 我們將在下一個版本中新增支援，擷取「開啟」、「點按」和「取消訂閱」事件的Smart Campaign執行資訊，以區別這些事件。

## 依裝置型別或裝置作業系統篩選時，為何許多量度會顯示零？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除了點按開啟率、開啟數、點按數和取消訂閱數之外，所有其他支援的量度都是傳遞事件或衍生自傳遞事件的比率。 由於裝置型別和裝置作業系統僅適用於參與量度，因此我們完全沒有資訊可顯示。 例如，在依裝置型別=行動裝置篩選時，詢問傳遞率是未定義的查詢，因為Marketo可能沒有收到基礎「傳送」和「已傳送」事件的任何參與量度。 我們正在探索從參與度量度套用裝置型別和裝置作業系統的方式，以取得包含參與和傳送度兩者的比率。

## 當某些電子郵件使用者端封鎖影像時，「電子郵件深入分析」會做什麼？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

一個常見的產業問題是越來越多的電子郵件使用者端預設關閉影像。 載入影像是記錄「開啟」的基礎。 使用者完全有可能收到包含已封鎖影像，但文字和連結完全可讀的電子郵件。 如果使用者遇到這種情況，並按一下該電子郵件中的連結，您最終可能會遇到點選事件的情況，但不會出現該電子郵件對應的「開啟」事件。 Marketo電子郵件深入分析會自動產生任何遺失的事件。 邏輯與Marketo對電子郵件效能報表以及收入總管中的電子郵件分析區域執行的操作相同。
