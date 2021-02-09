---
unique-page-id: 12983291
description: 瞭解收件者時區——行銷檔案——產品檔案
title: 瞭解收件者時區
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 瞭解收件者時區{#understanding-recipient-time-zone}

電子郵件和參與計畫可設定成根據收件者的時區傳送，因此不需要建立多個計畫——只要傳送一次，行銷人員就會自動保留電子郵件，直到當地時間正確為止。

>[!NOTE]
>
>收件者時區目前僅&#x200B;****&#x200B;適用於電子郵件內容。 它不適用於預設的參與計畫。

## 電子郵件程式{#email-programs}

當[計畫電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)時，有兩種主要方案：

1. 計畫在25小時內運行程式。
1. 計畫在未來（即下週）運行25小時以上。

為了適應每個時區，使用收件者時區排程的電子郵件程式會在世界上&#x200B;**first/eariest**&#x200B;時區的午夜開始執行(UTC +14:00)。

## 參與計畫{#engagement-programs}

當您[排程參與程式串流](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)且「收件者時區」處於活動狀態時，程式轉播將在UTC +14:00的午夜開始執行。 我們要求您在未來至少安排25小時（24小時+開始促銷活動的時間）進行首次演出，因為人們可能符合全球每個時區的演出資格。 目前以UTC +14:00開始處理，保證我們會在排程的日期和時間傳送電子郵件給符合此類廣播資格的每個人。

## 計算時區{#calculating-time-zone}

Marketo會根據人員的「城市」、「州」、「國家」或「郵遞區號」來計算時區。 如果我們無法根據這些值計算某人的時區，我們會回復到「推斷的城市」、「推斷的州」、「推斷的國家」和「推斷的郵遞區號」欄位。

如果我們只有&#x200B;****&#x200B;國家或&#x200B;****&#x200B;國家／地區，則：

* 對於三個或三個以下時區的國家，我們選擇中間時區。
* 對於兩個時區的州，我們選擇兩個時區中較早的。

如果我們仍無法從這些欄位的任意組合中判斷某人的時區，我們將&#x200B;**not**&#x200B;指派時區，而電子郵件會根據您的Marketo訂閱時區傳送。 因此，如果您的計畫排程在上午9:00 PDT，則沒有指定時區的人將在上午9:00 PDT收到電子郵件。

>[!NOTE]
>
>Marketto會在上述任何輸入欄位變更時自動重新計算人員的時區。

>[!MORELIKETHIS]
>
>* [計畫包含收件者時區的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [電子郵件計畫快速入門](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [與收件者時區排程參與計畫](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

