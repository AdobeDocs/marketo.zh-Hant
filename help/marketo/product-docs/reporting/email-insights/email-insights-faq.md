---
unique-page-id: 10100257
description: 電子郵件深入分析常見問題集 — Marketo檔案 — 產品檔案
title: 電子郵件洞察常見問題
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---

# 電子郵件洞察常見問題 {#email-insights-faq}

## 含有[!UICONTROL Email Insights]的比率量度與其他Marketo電子郵件報告之間是否有任何差異？ {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

可以。[!UICONTROL Email Insights]將參與量度與計算參與量度比率（開啟率、點按開啟率、取消訂閱率）時傳送之相同電子郵件的對應傳遞量度建立關聯。 例如，在[!UICONTROL Email Insights]中，檢視過去一週包含每日點按開啟率劃分的時間序列圖表時，我們現在會根據對應的傳送量度顯示開啟/點按/取消訂閱事件的真正相關比率。 這與Revenue Explorer中的行為形成對照，後者只是一切的總和。 [!UICONTROL Email Insights]提供更精確的參與率檢視。

## 為什麼[!UICONTROL Email Insights]只支援10個自訂維度？ {#why-does-email-insights-only-support-custom-dimensions}

對於許多使用案例，以10個額外的自訂維度擴充預設系統維度已足夠，並包括根據分段或計畫標籤的自訂維度。 我們計畫在未來允許客戶增加允許的自訂維度數量。

## 為何無法在指派後重複使用自訂維度槽？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

分配指定的自訂Dimension位置後，重新對應它會導致先前的資料在與新含義混合時產生錯誤。 因此，自訂Dimension位置可能無法重複使用。 此行為與其他量度分析工具(例如Google Analytics)的行為一致。

## [!UICONTROL Email Insights]是否支援Marketo Sales Insight電子郵件？ {#does-email-insights-support-marketo-sales-insight-emails}

可以。所有透過Marketo銷售分析傳送的電子郵件都包含在[!UICONTROL Email Insights]中。

## [!UICONTROL Email Insights]是否支援營運電子郵件？ {#does-email-insights-support-operational-emails}

可以。依預設，檢視和查詢會隱藏營運電子郵件。 不過，您可以在「個人設定」面板下變更此設定。

## [!UICONTROL Email Insights]是否擷取週期性排程或重新執行Smart Campaign電子郵件流程步驟？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

「是」與「否」。 在[!UICONTROL Email Insights]的初始版本中，所有電子郵件事件皆會擷取並可供任何週期性排程或重新執行的Smart Campaign存取。 但您無法區分該Smart Campaign的不同執行。 我們將在下一個版本中新增支援，以擷取「開啟」、「點按」和「取消訂閱」事件的Smart Campaign執行資訊，進而加以區分。

## 依裝置型別或裝置作業系統篩選時，為何許多量度會顯示零？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除了點按開啟率、開啟、點按和取消訂閱之外，所有其他支援的量度都是傳遞事件或衍生自傳遞事件的比率。 由於裝置型別和裝置作業系統僅適用於參與量度，因此我們完全沒有資訊可顯示。 例如，在依裝置型別=行動裝置篩選時詢問傳遞率是未定義的查詢，因為Marketo可能沒有收到基礎傳遞和已傳送事件的任何參與量度。 我們正在探索如何從參與量度套用裝置型別和裝置作業系統，以取得包含參與和傳送量度的比率。

## 當某些電子郵件使用者端封鎖影像時，[!UICONTROL Email Insights]會怎麼做？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

一個常見的產業問題是越來越多的電子郵件使用者端預設會關閉影像。 載入影像是記錄「開啟」的基礎。 使用者完全有可能收到含有已封鎖影像的電子郵件，但文字和連結完全可讀。 如果使用者遇到這個情況，並按一下該電子郵件中的連結，您最後會遇到點按事件的情況，但不會收到該電子郵件對應的「開啟」事件。 Marketo電子郵件深入分析會自動產生任何遺失的事件。 邏輯與Marketo對電子郵件效能報表以及Revenue Explorer中的電子郵件分析區域執行的操作相同。
