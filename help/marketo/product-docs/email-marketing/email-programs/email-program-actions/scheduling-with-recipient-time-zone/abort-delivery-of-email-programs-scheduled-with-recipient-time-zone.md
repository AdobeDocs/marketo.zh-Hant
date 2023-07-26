---
unique-page-id: 13795727
description: 中止傳送排程為收件者時區的電子郵件計畫 — Marketo檔案 — 產品檔案
title: 中止以收件者時區排程的電子郵件程式傳遞
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# 中止以收件者時區排程的電子郵件程式傳遞 {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

在緊急情況下，您可以中止已在啟用收件者時區的情況下開始執行的電子郵件程式傳遞。

由於使用收件者時區排程的電子郵件程式最多可以執行24小時，因此中止程式傳送將會取消該時間點之後的任何後續傳送。

1. 選取您要取消的電子郵件程式，然後按一下 **中止傳遞** 在「控制面板」的「核准」表徵圖下。

   ![](assets/ptz-abortdelivery.png)

1. 按一下「 」，確認您要取消傳遞 **中止**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. 取消後， **結果** 您的電子郵件程式的方格看起來會類似於下面的方格。 所有後續傳送均會被取消，並會在中顯示「電子郵件已軟退回」。 **活動型別** 欄。

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >取消的電子郵件將 **非** 顯示為軟退信 *直到* 原本排程在各自時區傳送的時間。 在此之前，他們仍會顯示為「傳送電子郵件」。

1. 在網格中，您可以按一下任何電子郵件來檢視活動詳細資訊。 對於已取消的傳送，詳細資料快顯視窗看起來會像這樣：

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [瞭解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [依收件者時區排程電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
