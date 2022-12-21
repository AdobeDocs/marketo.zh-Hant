---
unique-page-id: 12983291
description: 了解收件者時區 — Marketo檔案 — 產品檔案
title: 了解收件者時區
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 了解收件者時區 {#understanding-recipient-time-zone}

您可以根據收件者的時區來設定電子郵件和參與程式的傳送方式，而不需要建立多個程式，只要傳送一次，Marketo就會自動保留電子郵件，直到正確的當地時間為止。

>[!NOTE]
>
>收件者時區目前可運作 **僅限** 和電子郵件內容。 預設參與計畫將無法運作。

## 電子郵件方案 {#email-programs}

有兩種主要情況： [排程電子郵件方案](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. 將程式排程在接下來的25小時內執行。
1. 將計畫安排在未來運行超過25小時（即下週）。

為了適應每個時區，與收件者時區一起排程的電子郵件程式會在 **first/earlist** 世界時區（世界協調時+14:00）。

## 參與計畫 {#engagement-programs}

當您 [排程參與方案串流](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) 且收件者時區處於作用中狀態，程式轉播將在午夜(UTC +14:00)開始執行。 我們要求您在未來至少安排25小時（24小時+一些時間開始促銷活動）的首次演出，因為人們可能有資格在全球的每個時區參加。 現在以UTC +14:00開始處理，保證我們會針對符合此轉播資格的每個人，於排程日期和時間傳送電子郵件。

## 計算時區 {#calculating-time-zone}

Marketo會根據人員的「城市」、「州」、「國家」或「郵遞區號」來計算時區。 如果我們無法根據這些值計算某人的時區，我們會回復到「推斷的城市」、「推斷的州」、「推斷的國家」和「推斷的郵遞區號」欄位。

如果我們 **僅限** 國家/地區或 **僅限** 可用狀態：

* 對於時區數為三或三以下的國家，我們選取中時區。
* 對於具有兩個時區的州，我們會選取兩者中較早的。

如果我們仍無法從這些欄位的任何組合中判斷某個使用者的時區，我們會 **not** 指派時區，系統會根據您的Marketo訂閱時區傳送電子郵件。 因此，如果您的程式計畫在太平洋夏令時間上午9:00，則沒有分配時區的人員將在太平洋夏令時間上午9:00發送電子郵件。

>[!NOTE]
>
>Marketo會在上述任何輸入欄位變更時，自動重新計算人員的時區。

>[!MORELIKETHIS]
>
>* [使用收件者時區排程電子郵件方案](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [電子郵件計畫搶灘](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [與收件者時區排程參與方案](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

