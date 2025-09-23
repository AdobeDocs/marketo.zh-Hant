---
unique-page-id: 11383945
description: 瞭解Facebook離線轉換 — Marketo檔案 — 產品檔案
title: 了解 Facebook 離線轉換
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 2%

---

# 瞭解[!DNL Facebook]個離線轉換 {#understanding-facebook-offline-conversions}

Facebook銷售機會廣告行銷活動會產生銷售機會，並將其傳送到Marketo以用於行銷活動。 但是，如果無法檢視離線轉換，[!DNL Facebook]廣告商就無法知道哪些廣告最有效。 範例如下。

>[!NOTE]
>
>**範例**
>
>[!UICONTROL Facebook Lead Ads]執行三個廣告。
>
>* 廣告1產生20個銷售機會
>* 廣告2產生30個銷售機會
>* 廣告3產生50個銷售機會
>
>僅從這些數字來看，廣告3似乎最有效。
>
>但是，在Marketo端檢視資料時，畫面會呈現不同的情節。
>
>* 廣告1產生10個銷售
>* 廣告3產生2個銷售
>
>這表示廣告1雖然產生的銷售機會較少，但成功率為50%，而廣告3則幾乎完全無效。
>
>如果沒有離線轉換，廣告商可能會在Ad 3上投入更多資金。 有了離線轉換資料，廣告商可能會投資於廣告1。

您可以[設定Facebook離線轉換](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)，將離線廣告效能傳送給[!DNL Facebook]。

1. 確定您的[[!DNL Facebook] [!UICONTROL LaunchPoint]整合](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md)為最新狀態。
1. 將收入週期模型中的階段對應至[!DNL Facebook]上的離線轉換階段。
1. 當從[!DNL Facebook]銷售機會廣告產生[!DNL Facebook]銷售機會並到達對應的階段時，Marketo會每天透過安全且自動化的API將離線轉換資料傳送回[!DNL Facebook]多次。 資料會顯示在「[!DNL Facebook]廣告管理員」報表中。

>[!MORELIKETHIS]
>
>[設定 [!DNL Facebook] 離線轉換](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
