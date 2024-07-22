---
unique-page-id: 13795727
description: 中止傳送排程為收件者時區的電子郵件計畫 — Marketo檔案 — 產品檔案
title: 中止以收件者時區排程的電子郵件程式傳遞
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# 中止以收件者時區排程的電子郵件程式傳遞 {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

在緊急情況下，您可以中止已在啟用收件者時區的情況下開始執行的電子郵件程式傳遞。

由於使用收件者時區排程的電子郵件程式最多可以執行24小時，因此中止程式傳送將會取消該時間點之後的任何後續傳送。

1. 選取您要取消的電子郵件程式，然後按一下[控制檯]中[核准]方塊下的[中止傳遞] **。**

   ![](assets/ptz-abortdelivery.png)

1. 按一下&#x200B;**中止**，確認您要取消傳遞。

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. 取消之後，您電子郵件程式的&#x200B;**結果**&#x200B;方格將會看起來像下面的方格。 所有後續傳送都已取消，並將在&#x200B;**活動型別**&#x200B;欄中顯示為「電子郵件已退回」。

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >取消的電子郵件&#x200B;**不會**&#x200B;在原本排定在各自時區傳送的時間前&#x200B;*直到*&#x200B;顯示為軟退信。 在此之前，他們仍會顯示為「傳送電子郵件」。

1. 在網格中，您可以按一下任何電子郵件來檢視活動詳細資訊。 對於已取消的傳送，詳細資料快顯視窗看起來會像這樣：

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [瞭解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [排程收件者時區的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
