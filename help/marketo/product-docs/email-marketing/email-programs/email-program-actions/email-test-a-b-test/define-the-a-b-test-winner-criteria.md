---
unique-page-id: 2359545
description: 定義A/BTest優勝者標準 — Marketo文檔 — 產品文檔
title: 定義A/BTest贏家標準
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
source-git-commit: acea096990b834654b47c40b601ef2418069b9b5
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# 定義A/BTest贏家標準 {#define-the-a-b-test-winner-criteria}

當 [添加A/Btest](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;}到您的電子郵件程式，您需要選擇test類型， [安排A/Btest](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}，然後定義獲勝條件。 下面是如何決定哪封電子郵件會成功。

>[!PREREQUISITES]
>
>[添加A/BTest](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;

## 獲獎標準 {#winner-criteria}

1. 預設 **獲獎標準** 列出。

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>開啟</b></td>
   <td>當影像下載到電子郵件中時，開啟註冊。 即使您不包括影像，預設情況下，Marketo會在所有HTML電子郵件中插入單個跟蹤像素。</td>
   </tr>
   <tr>
   <td><b>按一下</b></td>
   <td>預設情況下，電子郵件中的連結中嵌入了跟蹤功能，使您能夠查看誰按一下了哪個連結、按一下了多少個總連結等。</td>
   </tr>
   <tr>
   <td><b>按一下以開啟%</b></td>
   <td>已開啟並在電子郵件中按一下連結的電子郵件的百分比。 這將測量電子郵件的關聯性和上下文，方法是：將唯一按一下的次數除以唯一開啟的次數，再乘以100將其顯示為百分比。</td>
   </tr>
   <tr>
   <td><b>項目分數</b></td>
   <td>的 <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">項目評分</a> 幫助您確定內容的有效性。</td>
   </tr>
   </table>

   >[!TIP]
   >
   >如果選擇「項目得分」，test至少需要運行24小時。 瞭解有關 [瞭解項目評分](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target=&quot;_blank&quot;}。

1. 也可以通過選擇「自定義轉換」並按一下「編輯」來自定義條件。

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >「自定義轉換」允許您使用觸發器和篩選器將任何事件作為轉換來選取。

1. 窗戶會開啟。 查找選項的觸發器，並將其拖到畫布中。

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. 定義觸發器。

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo將僅允許從此電子郵件程式發送電子郵件的人使用觸發器。 無需添加「已發送電子郵件」篩選器。

1. 按一下 **關閉**。

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   太好了！ 現在是時候決定勝者的決心了。

## 聲明贏家 {#declare-winner}

1. 從兩個可用選項中選擇一個。

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >如果你在 **日期/時間** A/Btest，您只能選擇 **手動**。

   A/Btest結束後，Marketo可以在預定時間自動發送獲勝的電子郵件，或者您可以查看結果並決定何時發送哪封電子郵件。

1. 「自動」功能強大，是預設選項。 按一下 **下一個**。

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >選擇 **手動** 會派test出去，等你宣佈獲勝。 您將收到結果報告。

完美！ 現在 [安排A/Btest](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}。
