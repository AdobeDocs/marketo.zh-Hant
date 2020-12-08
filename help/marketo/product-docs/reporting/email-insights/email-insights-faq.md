---
unique-page-id: 10100257
description: 電子郵件見解常見問答集——行銷人員檔案——產品檔案
title: 電子郵件見解常見問答集
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# 電子郵件見解常見問答集 {#email-insights-faq}

## 「電子郵件見解」和其他「行銷人員電子郵件」報告的比率指標之間是否有任何差異？ {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

是的。 「電子郵件見解」會將參與度量與計算參與度量比率（開放率、點按開放率、取消訂閱率）時傳送之相同電子郵件的對應傳送度量建立關聯。 例如，在「電子郵件分析」中，當查看過去一週的時間序列圖表及點按至開放率的每日劃分時，我們現在會根據對應的傳送量度，顯示開啟／點按／取消訂閱事件的真實關聯率。 這與「收入總管」中的行為形成鮮明對比，「收入總管」只是將所有內容總結。 「電子郵件見解」可提供更準確的參與率檢視。

## 為什麼「電子郵件見解」只支援10個自訂維度？ {#why-does-email-insights-only-support-custom-dimensions}

在許多使用案例中，將預設系統維度擴充為10個額外的自訂維度將綽綽有餘，並包含以區段或程式標籤為基礎的自訂維度。 未來，我們計畫允許客戶增加允許的自訂維度數目。

## 為什麼指派「自訂維度」槽後，無法重新使用這些槽？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

一旦分配了指定的「自訂維度」槽，重新映射將會導致先前的資料在混合新含義時產生錯誤。 因此，不得重新使用自訂維度槽。 此行為與其他量度分析工具（例如Google Analytics）一致。

## Email Insights是否支援Marketo Sales Insight電子郵件？ {#does-email-insights-support-marketo-sales-insight-emails}

是的。 所有透過Marketor Sales Insights傳送的電子郵件都包含在「電子郵件見解」中。

## 「電子郵件見解」是否支援運營電子郵件？ {#does-email-insights-support-operational-emails}

是的。 依預設，操作電子郵件會隱藏在檢視和查詢中。 不過，您可以在「個人設定」面板下變更此設定。

## 「電子郵件見解」會擷取定期排程或重新執行「智慧型促銷活動」電子郵件流程步驟嗎？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

是和否。 在初次發行的「電子郵件見解」中，所有電子郵件事件都可擷取，並可針對任何週期性的計畫或重新執行「智慧型促銷活動」存取。 但您無法區分該智慧型促銷活動的不同執行。 我們將在下一版中新增支援，以擷取「開啟」、「按一下」和「取消訂閱」事件的「智慧型促銷活動」執行資訊，以區隔其他事件。

## 依裝置類型或裝置作業系統篩選時，為什麼許多量度顯示為零？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除了點按至開放率、開啟、點按和取消訂閱之外，所有其他支援的度量皆為來自傳送事件的傳送事件或比率。 由於「裝置類型」和「裝置作業系統」僅適用於「參與」度量，因此我們根本沒有可顯示的資訊。 例如，依裝置類型=行動篩選時，要求傳送率的查詢未定義，因為Marketo不會收到任何基礎傳送和傳送事件的參與度量。 我們正在探討如何從參與量度套用裝置類型和裝置作業系統，以取得包含參與和傳送量度的比率。

## 當某些電子郵件客戶封鎖影像時，「電子郵件見解」會做什麼？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

一個常見的行業問題是，越來越多的電子郵件客戶預設關閉映像。 載入影像是記錄「開啟」的基礎。 使用者完全可能會收到電子郵件，其中包含封鎖的影像，但文字和連結完全可讀。 如果使用者經歷此情況，並點按該電子郵件中的連結，您最後會出現「點按」事件的情形，但該電子郵件沒有對應的「開啟」事件。 Marketo Email Insights會自動產生任何遺漏的事件。 邏輯與Marketto對「電子郵件效能」報表以及「收入總管」中「電子郵件分析」區域執行此動作的方式相同。
