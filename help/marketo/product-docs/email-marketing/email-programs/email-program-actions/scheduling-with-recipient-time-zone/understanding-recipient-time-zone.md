---
unique-page-id: 12983291
description: 瞭解收件者時區 — Marketo檔案 — 產品檔案
title: 瞭解收件者時區
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# 瞭解收件者時區 {#understanding-recipient-time-zone}

電子郵件和參與計畫可設定為根據收件者的時區傳送，無需建立多個計畫，只需傳送一次，Marketo會自動保留電子郵件，直到正確的當地時間為止。

>[!NOTE]
>
>收件者時區目前有效 **僅限** 包含電子郵件內容。 無法用於預設的參與計畫。

## 電子郵件程式 {#email-programs}

發生以下情況時，有兩種主要情況 [排程電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)：

1. 排程程式在未來25小時內執行。
1. 排程程式在未來（亦即下週）執行超過25小時。

為了適應每個時區，使用收件者時區排程的電子郵件程式會在 **第一個/最早的** 世界時區(UTC +14:00)。

## 參與計畫 {#engagement-programs}

當您 [排程參與方案資料流](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) 且收件者時區為作用中，程式轉換將在UTC +14:00的午夜開始執行。 我們要求您安排未來至少25小時進行第一次點播（24小時+開始促銷活動的時間），因為全球各地每個時區的人們都可能有資格參加點播。 目前以UTC +14:00開始處理，保證我們會在排程的日期和時間，為每位符合此演出資格的人傳送電子郵件。

## 計算時區 {#calculating-time-zone}

Marketo會根據個人的城市、州/省、國家/地區或郵遞區號計算時區。 如果我們無法從這些值計算某人的時區，我們會恢復為推斷的城市、推斷的州、推斷的國家和推斷的郵遞區號欄位。

若我們有 **僅限** 國家或地區 **僅限** 可用狀態：

* 對於時區少於三個的國家/地區，我們選取中間時區。
* 對於具有兩個時區的狀態，我們選取兩個時區中較早的一個。

如果我們仍然無法從這些欄位的任意組合中判斷某人的時區，我們將 **not** 指派時區，系統將根據您的Marketo訂閱時區傳送電子郵件。 因此，如果您的計畫是上午9:00 PDT，則未指派時區的人員將在上午9:00 PDT收到電子郵件。

>[!NOTE]
>
>當以上任何輸入欄位變更時，Marketo會自動重新計算人員的時區。

>[!MORELIKETHIS]
>
>* [使用收件者時區排程電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [電子郵件計畫的開端](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [依收件者時區排程參與方案](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
