---
unique-page-id: 12983280
description: 發行說明 — 17年秋季 — Marketo檔案 — 產品檔案
title: 發行說明 — 2017年秋季
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# 發行說明：』17年秋季 {#release-notes-fall}

』17年秋季版包含下列功能。 查看您的Marketo版本以了解功能可用性。

請按一下標題連結，以檢視每項功能的詳細文章。 注意：此版本包含的部分功能沒有相關文章。 如果主題有多個子標題，則連結會放在該處。

## 系統可靠性 {#system-reliability}

我們進一步改善了核心的Marketo基礎設施，包括更好的順序、更少的不匹配以及改善Munchkin穩定性。

## SFDC同步效能 {#sfdc-sync-performance}

利用Marketo和Salesforce之間更豐富、更快速的同步。 需要對帳戶或銷售機會進行大量更新的資料更改可以拆分到並行隊列，以避免積壓。 事件和任務現在的同步速度也提高了50%。

## Analytics效能改善 {#analytics-performance-improvements}

最近基礎架構的改善，讓Marketo報告和分析工具的正常運作時間和穩定性得以提高，讓您能更快速地建立臨機報告。

## [收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

透過這項新功能，您現在可以根據當地時區保留並傳送電子郵件。 您可以將電子郵件和參與程式設定為在收件者的時區傳送，而不需要建立多個程式，只要傳送一次，Marketo就會自動保留電子郵件，直到正確的當地時間為止。 全域使用單一方案，提升電子郵件量度、觀察本機實務，並節省時間。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>如果您尚未在電子郵件和參與計畫上啟用收件者時區，請不要驚慌！ 我們正在逐步為所有客戶啟用此功能。

## [依區段檢閱範例電子郵件](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo有新選項，可在傳送範例電子郵件供檢閱時挑選區段。 您不再需要手動判斷銷售機會屬於哪個區段，讓傳送包含動態內容的電子郵件至不同區段變得更輕鬆。

## [linkedIn主要一般自訂問題](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

自訂您的LinkedIn銷售機會代表表單以收集自訂銷售機會屬性。 您現在可以針對每個表單提出最多三個自訂問題、從單行文字輸入或多選題中選擇，然後對應回Marketo銷售機會欄位。

## Slack整合 {#slack-integration}

我們發佈兩項功能，作為新Slack整合的一部分：

* 系統通知：取得Marketo例項中重要事件的Slack通知，例如目前促銷活動狀態和任何需要立即注意的問題的警報。
* 有趣的時刻：當Marketo Insight由來自銷售帳戶的已知個人觸發時，銷售機會擁有者可透過Slack收到通知。 通知包括銷售機會資訊以及銷售帳戶的詳細資訊。

## ABM增強功能 {#abm-enhancements}

**[顯示沒有聯繫人的帳戶](https://docs.marketo.com/x/fKCt)**

Marketo ABM現在會同步並顯示CRM帳戶，而不需聯絡人。 包括沒有以前銷售或市場營銷歷史記錄的新帳戶，並通過將後續銷售線索匹配到帳戶來跟蹤進度。

## ContentAI Analytics {#contentai-analytics}

**[新的ABM帳戶清單篩選器](https://docs.marketo.com/x/1BPG)**

查看並比較ABM帳戶清單中的內容效能，以優化現有內容。 ContentAI會顯示：

* 已檢視的排名內容
* 最上層轉換的內容
* 行銷活動的AI支援建議內容

## 網頁個人化增強功能 {#web-personalization-enhancements}

**[Web促銷活動的代號](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Token現在可用於網頁促銷活動。 運用代號來提供個人化訊息和內容，以提升您對網頁行銷活動的參與度。

![](assets/image2017-11-16-11-3a25-3a7.png)

**[在Web Campaign編輯器中設計Studio影像](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

在Marketo中跨多個管道重複使用創意資產和影像，節省時間。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 整合  {#integration}

**[電子郵件預覽API](https://developers.marketo.com/rest-api/assets/emails/)**

您現在可以在Marketo外部遠端預覽電子郵件，簡化電子郵件內容本地化的程式並減少錯誤。

**[取代HTMLAPI](https://developers.marketo.com/rest-api/assets/emails/)**

開發人員可以遠端更新電子郵件資產的HTML內容，讓他們在單一系統內工作以維護資產。
