---
unique-page-id: 11383945
description: 瞭解Facebook離線轉換 — Marketo檔案 — 產品檔案
title: 瞭解Facebook離線轉換
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 瞭解Facebook離線轉換 {#understanding-facebook-offline-conversions}

facebook銷售機會廣告行銷活動會產生銷售機會，並將其傳送至Marketo，以用於行銷活動。 但是，如果沒有離線轉換的可見度，Facebook廣告商就無法知道哪些廣告最有效。 範例如下。

>[!NOTE]
>
>**範例**
>
>facebook Lead Ads執行三個廣告。
>
>* 廣告1產生20個銷售機會
>* 廣告2產生30個銷售機會
>* 廣告3產生50個銷售機會
>
>僅從這些數字來看，廣告3似乎最有效。
>
>不過，在Marketo端檢視資料時，會出現不同的案例。
>
>* 廣告1產生10個銷售
>* 廣告3產生2個銷售
>
>這表示廣告1雖然產生的銷售機會較少，但成功率為50%，而廣告3則幾乎完全無效。
>
>如果沒有離線轉換，廣告商可能會將更多資金投資於廣告3。 有了離線轉換資料，廣告商將更有可能投資於廣告1。

您可以 [設定Facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) 傳送離線廣告效能至Facebook。

1. 確定您的 [facebook LaunchPoint整合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) 為最新狀態。
1. 將收入週期模型中的階段對應至Facebook上的離線轉換階段。
1. 當Facebook銷售機會從Facebook銷售機會廣告產生並到達對應的階段時，Marketo會透過安全且自動化的API，每天多次將離線轉換資料傳送回Facebook。 資料會顯示在「Facebook廣告管理員報表」中。

>[!MORELIKETHIS]
>
>[設定Facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
