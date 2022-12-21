---
unique-page-id: 10097202
description: 電子郵件計畫搶灘 — Marketo檔案 — 產品檔案
title: 電子郵件計畫搶灘
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 電子郵件計畫搶灘 {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[建立電子郵件方案](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

當您選擇電子郵件方案的日期/時間時，會決定方案何時開始處理。 如果您希望電子郵件在選取的時間啟動，「開始」會提前處理程式，以提供此選項。

## 標準頭開始 {#standard-head-start}

1. 按一下 **行銷活動**.

   ![](assets/one-1.png)

1. 尋找並選取您的電子郵件方案。

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start無法與A/B測試搭配使用。

1. 在「排程」方塊中，排程您的電子郵件，然後選取 **開始** 框。

   ![](assets/three-1.png)

   選擇「開始前」後，程式將在計畫時間前大約12小時開始處理。 處理開始後，程式即會鎖定。

   >[!CAUTION]
   >
   >在程式鎖定後取消訂閱的對象仍會收到電子郵件。 建議您調整取消訂閱通知，以反映取消訂閱可能需要1至2個工作天的時間才能處理。

1. 按一下 **核准方案**.

   ![](assets/four-1.png)

   方案核准後，您可能會在「核准」方塊上看到四種不同的狀態。

   * **等待運行：** 在方案通過後。
   * **處理已開始，等待運行：** 正在處理。
   * **處理已完成，等待運行：** 處理已完成，電子郵件現在正等待排程的啟動時間。
   * **已完成：** 程式已完成。

   >[!TIP]
   >
   >在程式鎖定後但在電子郵件發送前要取消嗎？ 沒問題！ 只需按一下 **中止程式** 在「批准」表徵圖的右下側。

   >[!NOTE]
   >
   >如果您在排程執行時間前不到12小時取消核准電子郵件程式，但之後又改變主意，則需要選取新日期/時間，在核準時至少要提前12小時。

## 從收件者時區開始 {#head-start-with-recipient-time-zone}

我們現有的「搶先」功能要求該計畫至少提前12小時安排。 這對收件者時區有何意義？ 回想一下，當「收件者時區」處於作用中狀態時，我們會在最早時區的午夜(UTC +14:00)開始執行電子郵件程式。 所以，為了 **both** 頭開始和收件者時區，需要排程方案 **比最早時區提前至少12小時(UTC +14:00)**.)

這表示，如果您在美國/洛杉磯，且想同時啟用「搶先」和「收件者時區」，則需要排程方案 **34小時** 事先。 我們怎麼得到這個號碼的？

![](assets/image2017-12-5-13-3a11-3a46.png)

[深入了解](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) 關於如何使用收件者時區排程電子郵件方案的資訊。

>[!MORELIKETHIS]
>
>* [排程您的電子郵件方案](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [使用收件者時區排程電子郵件方案](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [了解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

