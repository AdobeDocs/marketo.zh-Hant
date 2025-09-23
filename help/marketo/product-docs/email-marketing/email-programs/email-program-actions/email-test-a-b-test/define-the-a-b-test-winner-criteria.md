---
unique-page-id: 2359545
description: 定義A/B測試獲勝者條件 — Marketo檔案 — 產品檔案
title: 定義 A/B 測試勝出條件
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 21%

---

# 定義 A/B 測試勝出條件 {#define-the-a-b-test-winner-criteria}

當[將A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}新增至您的電子郵件程式時，您必須挑選測試型別，[排程A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}，然後定義獲勝者條件。 以下說明如何決定哪封電子郵件入選。

>[!PREREQUISITES]
>
>[新增A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## 獲勝者條件 {#winner-criteria}

1. 預設&#x200B;**[!UICONTROL Winner Criteria]**&#x200B;選項會先列出。

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>[!UICONTROL Opens]</b></td>
   <td>將影像下載到電子郵件中時，開啟的登入會進行。 即使不包含影像，根據預設，Marketo也會在所有HTML電子郵件中插入單一追蹤畫素。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Clicks]</b></td>
   <td>預設情況下，電子郵件中的連結會嵌入追蹤功能，讓您可以查看誰點按過哪個連結、總共點按了多少個連結等。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Click to Open] %</b></td>
   <td>電子郵件被開啟而且內含連結被點按的百分比。此數值將不重複點按次數除以不重複開啟次數，然後乘以 100 來用百分比呈現，可衡量電子郵件的相關性和內容。</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Engagement Score]</b></td>
   <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">參與分數</a>可協助您判斷內容的有效性。</td>
   </tr>
   </table>

   >[!TIP]
   >
   >如果您選擇參與分數，測試將需要執行至少24小時。 深入瞭解[瞭解參與分數](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}。

1. 您也可以選取&#x200B;**[!UICONTROL Custom Conversion]**&#x200B;並按一下&#x200B;**[!UICONTROL Edit]**&#x200B;來自訂條件。

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >自訂轉換可讓您使用觸發器和篩選器挑選任何事件作為轉換。

1. 視窗隨即開啟。 找出您選擇的觸發器，並將其拖曳至畫布中。

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. 定義觸發器。

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo僅允許從這個電子郵件程式傳送電子郵件之人員的觸發器/篩選器，因此不需要新增「已傳送電子郵件」篩選器。 此外，使用電子郵件相關的觸發器/篩選器時，請務必使用「is any」作為運運算元。

1. 按一下「**[!UICONTROL Close]**」。

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   太棒了！ 現在該決定如何決定獲勝者了。

## 宣告贏家 {#declare-winner}

1. 從兩個可用選項中選擇一個。

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >如果您正在進行&#x200B;**日期/時間** A/B測試，則只能選擇&#x200B;**[!UICONTROL Manual]**。

   A/B測試完成後，Marketo可以在排程的時間自動傳送成功電子郵件，或者您可以檢閱結果並決定哪封電子郵件何時送出。

1. 「自動」很棒，而且是預設選項。 只需按一下&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >選擇&#x200B;**[!UICONTROL Manual]**&#x200B;將會傳送測試並等待您宣告獲勝者。 您將會收到結果的報告。

完美！ 現在[排程A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}。
