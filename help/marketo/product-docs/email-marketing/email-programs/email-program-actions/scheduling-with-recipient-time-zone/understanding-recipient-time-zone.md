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

電子郵件和參與計畫可設定為根據收件者的時區傳送，因此無需建立多個計畫，只需傳送一次，Marketo會自動保留電子郵件，直到正確的當地時間為止。

>[!NOTE]
>
>收件者時區目前有效 **僅限** 包含電子郵件內容。 無法用於預設的參與計畫。

## 電子郵件程式 {#email-programs}

發生以下情況時有兩種主要情況 [排程電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)：

1. 排程程式在未來25小時內執行。
1. 排程程式在未來（亦即下週）執行25小時以上。

為了因應每個時區，以收件者時區排程的電子郵件程式會在的午夜開始執行。 **第一個/最早的** 全球時區(UTC +14:00)。

## 參與計畫 {#engagement-programs}

當您 [排程參與方案流](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) 收件者時區啟用時，程式轉換將在UTC +14:00的午夜開始執行。 我們要求您至少將未來的25小時（24小時+開始行銷活動的時間）排程為第一個演員，因為全球每個時區的人可能有資格參加演員。 目前以UTC +14:00開始處理，保證我們將在排程的日期和時間傳送電子郵件，給符合此演出資格的每個人。

## 正在計算時區 {#calculating-time-zone}

Marketo會根據人員的城市、州、國家/地區或郵遞區號計算時區。 如果我們無法從這些值計算某人的時區，我們會還原為推斷的城市、推斷的州、推斷的國家/地區和推斷的郵遞區號欄位。

若我們有 **僅限** 國家/地區或 **僅限** 可用狀態：

* 對於時區少於三個的國家/地區，我們選取中間時區。
* 對於具有兩個時區的狀態，我們選取兩個時區中較早的一個。

如果我們仍然無法從這些欄位的任意組合判斷某人的時區，我們將 **非** 指派時區，系統將根據您的Marketo訂閱時區傳送電子郵件。 因此，如果您的方案排程為太平洋夏季時間上午9:00，則未指派時區的人員將在太平洋夏季時間上午9:00收到電子郵件。

>[!NOTE]
>
>當以上任何輸入欄位變更時，Marketo會自動重新計算人員的時區。

>[!MORELIKETHIS]
>
>* [依收件者時區排程電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [電子郵件程式快速入門](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [依收件者時區排程參與方案](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
