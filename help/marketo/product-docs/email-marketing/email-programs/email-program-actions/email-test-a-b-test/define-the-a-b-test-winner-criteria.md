---
unique-page-id: 2359545
description: 定義A/B測試成功者標準——行銷人員檔案——產品檔案
title: 定義A/B測試成功者標準
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# 定義A/B測試成功者標準{#define-the-a-b-test-winner-criteria}

當[將A/B測試](add-an-a-b-test.md)新增至您的電子郵件程式時，您需要選擇測試類型[排程A/B測試](schedule-the-a-b-test.md)，然後定義成功者標準。 以下說明如何決定哪些電子郵件能贏。

>[!PREREQUISITES]
>
>* [新增A/B測試](add-an-a-b-test.md)

>



## 成功者條件{#winner-criteria}

1. 預設的&#x200B;**成功者標準**&#x200B;選項會先列出。

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **開啟** | 開啟會在影像下載至電子郵件時註冊。 即使您未包含影像，依預設，Market會將單一追蹤像素插入所有HTML電子郵件。 |
   |---|---|
   | **點按次數** | 依預設，電子郵件中的連結會內嵌追蹤，讓您查看誰點按了哪個連結、點按了多少個連結，等等。 |
   | **按一下以開啟%** | 已開啟且已點按電子郵件連結的電子郵件百分比。 這會測量電子郵件的相關性和內容，方法是取唯一點按次數除以唯一開啟次數，再乘以100以百分比顯示。 |
   | **參與分數** | [參與分數](http://docs.marketo.com/display/DOCS/Understanding+the+Engagement+Score)可協助您判斷內容的效果。 |

   >[!TIP]
   >
   >如果您選擇「參與分數」，則測試至少需要執行24小時。 進一步瞭解[瞭解參與分數](../../../../../product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md)。

   您也可以選擇「自訂轉換」並按一下「編輯」，自訂標準。
   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >「自訂轉換」可讓您使用觸發器和篩選器，選擇任何事件做為轉換。

   窗戶會開啟。 尋找您選擇的觸發器，並拖曳至畫布中。
   ![](assets/image2014-9-12-15-3a52-3a18.png)

   >[!NOTE]
   >
   >**深入探討**
   >
   >
   >進一步瞭解[智慧型清單和靜態清單](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)。

   定義觸發器。
   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo僅允許從此電子郵件程式傳送電子郵件的人員觸發。 不需要新增「已傳送電子郵件」篩選。

   按一下「關閉」。
   ![](assets/image2014-9-12-15-3a53-3a36.png)

   太好了！ 現在，是時候決定如何確定贏家了。

## 宣告成功者{#declare-winner}

1. 選擇兩個可用選項之一。

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >如果您正在執行&#x200B;**日期／時間** A/B測試，則只能選擇&#x200B;**手動**。

   A/B測試結束後，Marketo可以在排程的時間自動傳送成功的電子郵件，或者您可以檢閱結果，並決定何時送出哪封電子郵件。

1. 自動是絕佳的，是預設選項。 只要按一下「下一步」，即可。****

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >選擇&#x200B;**Manual**&#x200B;將發送測試並等待您聲明成功者。 您將會收到結果報告。

   [排程A/B測試](schedule-the-a-b-test.md)

完美！ 現在，讓我們。