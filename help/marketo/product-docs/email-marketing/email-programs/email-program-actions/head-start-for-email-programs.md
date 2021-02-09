---
unique-page-id: 10097202
description: 電子郵件計畫快速入門——行銷檔案——產品檔案
title: 電子郵件計畫快速入門
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 電子郵件程式快速入門{#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[建立電子郵件方案](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

當您選擇電子郵件程式的日期／時間時，會決定程式何時開始處理。 如果您希望電子郵件在選定時間啟動，Head Start會提前處理程式，為您提供此選項。

## 標準頭開始{#standard-head-start}

1. 按一下「行銷活動」**。**

   ![](assets/one-1.png)

1. 尋找並選取您的電子郵件方案。

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start不能用於A/B測試。

1. 在「排程」方塊中，排程您的電子郵件，然後選取「開始前」方塊。****

   ![](assets/three-1.png)

   在選擇「開始前」後，該程式將在預定時間前大約12小時開始處理。 一旦處理開始，程式即被鎖定。

   >[!CAUTION]
   >
   >在程式鎖定後取消訂閱的觀眾，仍會收到電子郵件。 我們建議您調整取消訂閱通知，以反映取消訂閱可能需要1-2個工作天才能處理。

1. 按一下&#x200B;**批准程式**。

   ![](assets/four-1.png)

   方案核准後，您在「核准」方塊上會看到四種不同的狀態。

   * **等待運行：** 程式獲得批准後。
   * **處理已開始，等待運行：處** 理正在進行中。
   * **處理完成，等待執行：處** 理完成，電子郵件現在等待排程的啟動時間。
   * **完成：程** 式完成。

   >[!TIP]
   >
   >想要在程式鎖定後取消，但電子郵件傳送之前取消？ 沒問題！ 只要按一下「核准」方塊右下方的「中止程式」(Abort Program)。****

   >[!NOTE]
   >
   >如果您在電子郵件程式排程執行時間前不到12小時取消核准，但是改變心意，則必須選擇新的日期／時間，這至少比您核準時提前12小時。

## 從收件者時區{#head-start-with-recipient-time-zone}開始

我們現有的Head Start功能要求計畫至少提前12小時完成。 這對收件者時區意味著什麼？ 請記住，當「收件者時區」處於活動狀態時，我們會在最早時區的午夜(UTC +14:00)開始運行電子郵件程式。 因此，要啟用&#x200B;**兩個**&#x200B;頭開始時區和接收時區，需要在最早時區之前至少安排&#x200B;**12小時(UTC +14:00**)。

這表示如果您在美國／洛杉磯，並想要同時啟用「開始前」和「接收者時區」，則需要事先安排計畫&#x200B;**34小時**。 我們怎麼得到這個號碼的？

![](assets/image2017-12-5-13-3a11-3a46.png)

[進一](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) 步瞭解如何使用收件者時區排程電子郵件方案。

>[!MORELIKETHIS]
>
>* [排程您的電子郵件方案](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [計畫包含收件者時區的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [瞭解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

