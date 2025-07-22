---
unique-page-id: 10097202
description: 電子郵件計畫快速入門 — Marketo檔案 — 產品檔案
title: 電子郵件程式快速入門
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 電子郵件程式快速入門 {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[建立電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

當您選擇電子郵件程式的日期/時間時，它會決定程式何時開始處理。 如果您希望電子郵件在選取的時間啟動，Head Start會預先處理計畫，為您提供該選項。

## 標準開端 {#standard-head-start}

1. 按一下「**[!UICONTROL Marketing Activities]**」。

   ![](assets/one-1.png)

1. 尋找並選取您的電子郵件程式。

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start不適用於A/B測試。

1. 在[!UICONTROL Schedule]圖磚中，排程您的電子郵件，然後選取&#x200B;**[!UICONTROL Head Start]**&#x200B;方塊。

   ![](assets/three-1.png)

   選取[!UICONTROL Head Start]後，程式將在排程時間前約12小時開始處理。 處理開始後，程式即會鎖定。

   >[!CAUTION]
   >
   >您的對象中，在方案鎖定後取消訂閱的任何人仍會收到電子郵件。 我們建議您調整取消訂閱通知，以反映取消訂閱可能需要1-2個工作日才能處理。

1. 按一下「**[!UICONTROL Approve Program]**」。

   ![](assets/four-1.png)

   方案核准後，您可能會在核准圖磚上看到四種不同的狀態。

   * **[!UICONTROL Waiting to run]：**&#x200B;方案核准後。
   * **[!UICONTROL Processing started, waiting to run]：**&#x200B;處理進行中。
   * **[!UICONTROL Processing finished, waiting to run]：**&#x200B;處理完成，電子郵件正在等待排定的啟動時間。
   * **[!UICONTROL Finished]：**&#x200B;程式已完成。

   >[!TIP]
   >
   >想要在程式鎖定後但在電子郵件傳送前取消？ 沒問題！ 只要按一下[核准]方塊右下角的&#x200B;**[!UICONTROL Abort Program]**&#x200B;即可。

   >[!NOTE]
   >
   >如果您在電子郵件程式排定的執行時間前12小時內取消核准該程式，但後來改變心意，您將需要選擇至少比核準時提前12小時的新日期/時間。

## 以收件者時區開頭的標題 {#head-start-with-recipient-time-zone}

我們現有的「開門即用」功能要求程式至少提前12小時排程。 這對收件者時區有何意義？ 回想一下，當收件者時區作用中時，我們會在最早時區的午夜開始執行電子郵件程式(UTC +14:00)。 因此，若要啟用&#x200B;**兩者**&#x200B;開始時間和收件者時區，程式需要排程在最早時區之前&#x200B;**至少12小時(UTC +14:00**)。

這表示如果您在美洲/洛杉磯，並且想要同時啟用開頭和收件者時區，您需要提前&#x200B;**34小時**&#x200B;排程程程式。 我們如何取得這個號碼？

![](assets/image2017-12-5-13-3a11-3a46.png)

[進一步瞭解](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)如何排程收件者時區的電子郵件程式。

>[!MORELIKETHIS]
>
>* [排程您的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [排程收件者時區的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [瞭解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
