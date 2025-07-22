---
unique-page-id: 2359476
description: 使用電子郵件程式控制面板 — Marketo檔案 — 產品檔案
title: 使用電子郵件程式控制面板
exl-id: 47c1925a-144b-4277-a08d-1af660ed3d50
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 使用電子郵件程式控制面板 {#use-the-email-program-dashboard}

檢視您的電子郵件程式使用此儀表板檢視的執行方式。

>[!CAUTION]
>
>為獲得準確的報告，請避免&#x200B;_重複使用電子郵件程式的_&#x200B;電子郵件，方法是在智慧行銷活動中參考該電子郵件，或將資產從已啟動的電子郵件程式移至新的電子郵件程式。 這麼做會彙總該電子郵件附加之每個報告控制面板中的所有資料。 如果您需要重複使用電子郵件，請改為複製[它](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-an-asset-in-a-program.md){target="_blank"}，因為這樣會複製電子郵件，但會建立具有新電子郵件識別碼的新電子郵件。

>[!NOTE]
>
>如果您的方案有A/B測試，請檢視[電子郵件方案儀表板 — A/B測試檢視](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}。

![](assets/image2014-9-12-14-3a12-3a56.png)

>[!NOTE]
>
>此檢視中的所有資料都是彙總的（包括A/B測試以及最終的電子郵件傳送）。

## 電子郵件傳送 {#email-send}

您可以在此處檢視已傳送、已退回及已傳遞的電子郵件數量。

![](assets/image2014-9-12-14-3a13-3a3.png)

>[!NOTE]
>
>由於電子郵件傳遞能力標準超出Marketo的控制，因此「已退回」和「已傳遞」統計資料僅為近似值，且不具準確性。

## 開啟次數/點按次數 {#opens-clicks}

此圖表顯示執行電子郵件程式後，特定時段內開啟/點按的電子郵件數目。

![](assets/image2014-9-12-14-3a13-3a7.png)

>[!TIP]
>
>請留意開啟/點按次數會隨時間推移而減少的情況。

## 摘要 — 參與 {#summary-engagement}

這會顯示整體[參與分數](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}。

![](assets/image2014-9-12-14-3a13-3a11.png)

## 摘要 — 休息 {#summary-rest}

其餘的資料將顯示「開啟」、「點按」、「點按/開啟比例」和「取消訂閱」。

![](assets/image2014-9-12-14-3a13-3a15.png)

>[!TIP]
>
>上述範例中的&#x200B;**取消訂閱**&#x200B;率太小，以至Marketo放大顯示，讓您更上一層樓。 列內的第二個數字只是為了縮放而增加。

>[!NOTE]
>
>**定義**
>
>電子郵件收件者下載電子郵件的影像(包含Marketo插入的追蹤畫素)時，會計入&#x200B;**[!UICONTROL Opens]**。 如果收件者檢視電子郵件但選擇不下載其影像，則不會計為已開啟。 如果影像載入收件者的預覽窗格，這通常會計為開啟，但會根據電子郵件使用者端而有所不同。
>
>**[!UICONTROL Click to Open]**&#x200B;測量在電子郵件中同時開啟及有連結點按的電子郵件百分比。 我們採用不重複點按次數除以不重複開啟次數，然後乘以100以百分比顯示。

## 重新整理儀表板 {#refresh-dashboard}

若要檢視最新資料，只要按一下控制面板上的重新整理圖示即可。

![](assets/refreshicon.png)

>[!MORELIKETHIS]
>
>[使用電子郵件程式儀表板 — A/B測試檢視](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}
