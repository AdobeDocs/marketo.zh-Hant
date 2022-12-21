---
unique-page-id: 11383945
description: 了解Facebook離線轉換 — Marketo檔案 — 產品檔案
title: 了解Facebook離線轉換
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 了解Facebook離線轉換 {#understanding-facebook-offline-conversions}

Facebook Lead Ads促銷活動會產生銷售機會，並將其傳送至Marketo以用於行銷活動。 不過，若無法顯示離線轉換，Facebook廣告商將無法知道哪些廣告最有效。 舉個例子。

>[!NOTE]
>
>**範例**
>
>Facebook Lead Ads會執行三個廣告。
>
>* 廣告1產生20個銷售機會
>* 廣告2產生30個銷售線索
>* 廣告3產生50個銷售線索
>
>僅從這些資料來看，第3條似乎最有效。
>
>然而，當查看Marketo端的資料時，會發生不同的情況。
>
>* 廣告1產生10個銷售
>* 廣告3產生2個銷售
>
>這意味著，儘管創造的線索較少，但廣告1的成功率只有50%，而廣告3則幾乎毫無效果。
>
>若無離線轉換，廣告商可能會在廣告3上投入更多資金。 有了離線轉換資料，廣告商更可能投資於廣告1。

您可以 [設定Facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) 將離線廣告效能傳送至Facebook。

1. 請確定您的 [Facebook LaunchPoint整合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) 為最新。
1. 將收入週期模型中的階段對應至Facebook上的離線轉換階段。
1. 當Facebook Lead從Facebook Lead產生並達到對應階段時，Marketo會透過安全的自動化API每天將離線轉換資料傳回Facebook數次。 資料會顯示在Facebook廣告管理員報表中。

>[!MORELIKETHIS]
>
>[設定Facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
