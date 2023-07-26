---
unique-page-id: 12983280
description: 發行說明–2017年秋季 — Marketo檔案 — 產品檔案
title: 發行說明 — 2017年秋季
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# 發行說明： 2017年秋季 {#release-notes-fall}

以下功能包含在2017年秋季發行版本中。 檢查您的Marketo版本是否有功能可用。

請按一下標題連結以檢視每個功能的詳細文章。 注意：此版本包含的部分功能沒有相關文章。 如果主題有多個副標題，連結就會放在那裡。

## 系統可靠性 {#system-reliability}

我們已進一步改善核心Marketo基礎架構，包括更優異的排序、更少的不相符，以及更佳的Munchkin穩定性。

## SFDC同步效能 {#sfdc-sync-performance}

利用Marketo和Salesforce之間更豐富且更快速的同步處理。 需要大量更新帳戶或銷售機會的資料變更，可分割為平行佇列以避免積壓。 事件和任務同步速度現在也加快了50%。

## Analytics效能改善 {#analytics-performance-improvements}

最近的基礎架構改善專案，可提高Marketo報告與分析工具的運作時間和穩定性，讓您更快建立隨選報告。

## [收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

透過這項新功能，您現在可以根據當地時區保留及傳送電子郵件。 電子郵件和參與計畫可設定為在收件者的時區傳送，因此無需建立多個計畫，只需傳送一次，Marketo會自動保留電子郵件，直到正確的當地時間為止。 提升電子郵件量度、觀察本機實務，並在全域使用單一程式來節省時間。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>如果您還無法在電子郵件和參與計畫上啟用收件者時區，請勿驚慌！ 我們正在逐步為所有客戶啟用此功能。

## [依區段檢閱範例電子郵件](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

傳送範例電子郵件以供檢閱時，Marketo有新選項可挑選區段。 您不再需要手動判斷銷售機會屬於哪個區段，更輕鬆地傳送包含動態內容的電子郵件至不同區段。

## [linkedIn銷售機會一般自訂問題](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

自訂您的LinkedIn銷售機會一般表單，以收集自訂銷售機會屬性。 您現在可以在每個表單中詢問最多三個自訂問題、從單行文字輸入或多選問題中進行選擇，並對應回Marketo潛在客戶欄位。

## Slack整合 {#slack-integration}

我們發行了兩項功能，作為新Slack整合的一部分：

* 系統通知：取得有關Marketo執行個體中重要事件的Slack通知，例如有關目前行銷活動狀態的警示以及任何需要立即關注的問題。
* 有趣的時刻：當銷售帳戶中的已知個人觸發Marketo Insight時，系統會透過Slack通知潛在客戶擁有者。 通知包括潛在客戶資訊以及銷售帳戶的相關細節。

## ABM增強功能 {#abm-enhancements}

**[顯示沒有連絡人的帳戶](https://docs.marketo.com/x/fKCt)**

Marketo ABM現在會同步並顯示沒有連絡人的CRM帳戶。 納入沒有先前銷售或行銷歷史記錄的新帳戶，並將後續銷售線索與帳戶比對以追蹤進度。

## ContentAI分析 {#contentai-analytics}

**[新增ABM帳戶清單篩選器](https://docs.marketo.com/x/1BPG)**

檢視及比較不同ABM帳戶清單的內容效能，將現有內容最佳化。 ContentAI會顯示：

* 最常檢視的內容
* 排名在前的轉換內容
* AI支援的行銷活動建議內容

## Web Personalization增強功能 {#web-personalization-enhancements}

**[網頁行銷活動的代號](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Token現在可用於網頁行銷活動。 運用代號來提供個人化訊息和內容，以提升網站行銷活動的參與度。

![](assets/image2017-11-16-11-3a25-3a7.png)

**[在Web Campaign編輯器中設計工作室影像](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

在Marketo中跨多個管道重複使用創意資產和影像，以節省時間。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 整合  {#integration}

**[電子郵件預覽API](https://developers.marketo.com/rest-api/assets/emails/)**

您現在可以在Marketo外部遠端預覽電子郵件，簡化電子郵件內容本地化的程式，並減少錯誤。

**[取代HTML API](https://developers.marketo.com/rest-api/assets/emails/)**

開發人員可從遠端更新電子郵件資產的HTML內容，讓他們能在單一系統中工作，以維護資產。
