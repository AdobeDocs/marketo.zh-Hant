---
unique-page-id: 10100257
description: 電子郵件深入分析常見問題集 — Marketo檔案 — 產品檔案
title: 電子郵件深入分析常見問題集
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 電子郵件深入分析常見問題集 {#email-insights-faq}

## 「電子郵件分析」與其他Marketo電子郵件報表的比率量度之間是否有任何差異？ {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

是. 「電子郵件前瞻分析」會針對計算參與量度比率時傳送的相同電子郵件，將參與量度與其對應的傳送量度關聯（開放率、點按開放率、取消訂閱率）。 例如，在「電子郵件前瞻分析」中，查看過去一週的時間序列圖表以及每日點按開放率的劃分時，我們現在會根據對應的傳送量度，顯示開啟/點按/取消訂閱事件的真正相關比率。 這與「收入總管」中的行為相反，「收入總管」只是總結所有內容。 電子郵件深入分析可提供更精確的參與率檢視。

## 為什麼「電子郵件分析」僅支援10個自訂Dimension? {#why-does-email-insights-only-support-custom-dimensions}

在許多使用案例中，使用10個額外的自訂維度擴充預設系統維度將非常充分，並包含以區段或方案標籤為基礎的自訂維度。 未來，我們計畫允許客戶增加允許的自訂Dimension數量。

## 為什麼在指派自訂Dimension位置後，我無法重新使用這些位置？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

分配了指定的自訂Dimension槽後，重新映射它會在與新含義混合時導致先前的資料產生錯誤。 因此，自訂Dimension位置可能不會重複使用。 此行為與其他量度分析工具(例如Google Analytics)一致。

## 「電子郵件前瞻分析」是否支援Marketo Sales Insight電子郵件？ {#does-email-insights-support-marketo-sales-insight-emails}

是. 所有透過Marketo Sales Insights傳送的電子郵件都會包含在電子郵件Insights中。

## 「電子郵件前瞻分析」是否支援操作電子郵件？ {#does-email-insights-support-operational-emails}

是. 預設情況下，操作電子郵件在查看和查詢中隱藏。 不過，您可以在「個人設定」面板下更改此設定。

## 「電子郵件前瞻分析」會擷取重複排程或重新執行的Smart Campaign電子郵件流程步驟嗎？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

是和否。 在Email Insights的初始發行中，所有電子郵件事件都會被擷取，並可供任何週期性的排程或重新執行的Smart Campaign存取。 但您無法區分該智慧行銷活動的不同執行。 我們將在下一版中新增支援，以擷取「開啟」、「按一下」和「取消訂閱」事件的「智慧型促銷活動」執行資訊，以便加以區分。

## 依裝置類型或裝置作業系統篩選時，為何有許多量度顯示為零？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除了「點按開啟率」、「開啟」、「點按」和「取消訂閱」之外，所有其他支援的量度都是傳遞事件或從傳遞事件衍生的比率。 由於「裝置類型」和「裝置作業系統」僅套用至「參與」量度，因此我們根本沒有可顯示的資訊。 例如，依裝置類型=行動裝置篩選時，這是一個未定義的查詢，因為Marketo不會收到基礎傳送和已傳送事件的任何參與量度。 我們正在探索從參與量度套用裝置類型和裝置作業系統，以了解包含參與和傳送量度的比率。

## 某些電子郵件用戶端封鎖影像時，「電子郵件分析」有什麼作用？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

一個常見的行業問題是，越來越多的電子郵件客戶端預設關閉映像。 載入影像是記錄開啟的基礎。 使用者完全可能會收到封鎖影像的電子郵件，但文字和連結完全可讀。 如果使用者經歷此情況，並點按了該電子郵件中的連結，您最後會出現「點按」事件的案例，但該電子郵件沒有對應的「開啟」事件。 Marketo Email Insights會自動產生任何遺漏的事件。 此邏輯完全等同於Marketo對「電子郵件效能」報表以及收入總管中的「電子郵件分析」區域執行此動作的方式。
