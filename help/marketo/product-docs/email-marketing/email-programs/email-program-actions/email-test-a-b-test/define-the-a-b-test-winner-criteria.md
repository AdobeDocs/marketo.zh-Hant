---
unique-page-id: 2359545
description: 定義A/B測試獲勝者條件 — Marketo檔案 — 產品檔案
title: 定義A/B測試獲勝者條件
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
source-git-commit: 67ae4605d541a475b42a5094a5588c469a9d975d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 定義A/B測試獲勝者條件 {#define-the-a-b-test-winner-criteria}

當 [新增A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;})，您需要選取測試類型， [排程A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}，然後定義獲勝者條件。 以下說明如何決定哪封電子郵件能成功。

>[!PREREQUISITES]
>
>[新增A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;}

## 獲勝者條件 {#winner-criteria}

1. 預設 **獲勝者條件** 會先列出選項。

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>開啟</b></td>
   <td>開啟會在影像下載至電子郵件時註冊。 即使您未包含影像，依預設，Marketo會在所有HTML電子郵件中插入單一追蹤像素。</td>
   </tr>
   <tr>
   <td><b>點按次數</b></td>
   <td>依預設，電子郵件中的連結內嵌了追蹤功能，可讓您查看誰點按了哪個連結、總共點按了多少個連結，等等。</td>
   </tr>
   <tr>
   <td><b>按一下以開啟%</b></td>
   <td>已開啟且已點按電子郵件中連結的電子郵件百分比。 此度量電子郵件的相關性和內容，方法是取不重複點按次數除以不重複開啟次數，然後乘以100將其顯示為百分比。</td>
   </tr>
   <tr>
   <td><b>參與分數</b></td>
   <td>此 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">參與分數</a> 可協助您判斷內容的效用。</td>
   </tr>
   </table>

   >[!TIP]
   >
   >如果您選擇「參與分數」，則測試至少需要執行24小時。 深入了解 [了解參與分數](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target=&quot;_blank&quot;}。

1. 您也可以選取「自訂轉換」並按一下「編輯」，以自訂您的條件。

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >「自訂轉換」可讓您使用觸發器和篩選器來挑選任何事件作為轉換。

1. 窗口會開啟。 尋找您選擇的觸發器，並將其拖曳至畫布中。

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. 定義觸發器。

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo僅允許從此電子郵件方案傳送電子郵件的使用者觸發器/篩選器，因此不需要新增「已傳送電子郵件」篩選器。 此外，使用電子郵件相關觸發器/篩選器時，請務必使用「is any」作為運算子。

1. 按一下 **關閉**。

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   太棒了！ 現在是時候決定獲勝者的下場了。

## 宣佈獲勝者 {#declare-winner}

1. 從兩個可用選項中選擇一個。

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >如果你在做 **日期/時間** A/B測試，您只能選擇 **手動**.

   A/B測試結束後，Marketo可以在排程時間自動傳送成功的電子郵件，或者您可以檢閱結果，決定何時送出哪封電子郵件。

1. 「自動」(automatic)是「令人讚不絕口」(awesome)，是預設選項。 按一下 **下一個**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >選擇 **手動** 會傳送測試，並等待您宣告成功者。 您將收到結果報告。

完美！ 現在，讓我們 [排程A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}。
