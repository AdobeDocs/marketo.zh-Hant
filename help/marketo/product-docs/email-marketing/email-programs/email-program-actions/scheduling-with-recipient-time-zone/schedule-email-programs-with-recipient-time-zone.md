---
unique-page-id: 12982903
description: 使用收件者時區排程電子郵件程式 — Marketo檔案 — 產品檔案
title: 使用收件者時區排程電子郵件程式
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# 使用收件者時區排程電子郵件程式 {#schedule-email-programs-with-recipient-time-zone}

在啟用「收件者時區」的情況下排程電子郵件程式時，有兩種可能的情況：

1. 排程程式執行 **範圍** 接下來的25小時
1. 排程程式執行 **更多** 超過未來25小時（即下週）

## 案例1:25小時內 {#scenario-within-hours}

假設您核准啟用了收件者時區的電子郵件方案，以及未來25小時內排程的傳送時間。 您的智慧清單中可能有人住在排程時間已過的時區。

在此案例中，我們可讓您決定如何處理此合格人員子集。 按一下旁邊的齒輪圖示 **收件者時區** 在 **排程** 電子郵件程式的動態磚。

![](assets/image2017-12-5-10-3a46-3a42.png)

這為您提供兩個選項：

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**定義**
>
>* **在收件者的時區中傳遞隔天**：如果電子郵件排定在星期二上午9:00發出，則居住於已過排定時間的時區的合格人員將在收到電子郵件 *星期三* 上午9:00
>
>* **使用程式的預設設定時間傳遞**：如果電子郵件排定在星期二上午9:00發出，則居住於已過排定時間的時區的合格人員將收到電子郵件 _根據您的訂閱時區設定_. 因此，若您的 [訂閱時區設定](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) 設為PDT美洲/洛杉磯，則這些收件者仍會在星期二上午9:00 （無論時間位於他們自己的時區）收到電子郵件。

>[!NOTE]
>
>[瞭解更多](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) 關於Marketo如何計算收件者的時區。

讓我們更詳細地考慮此情境。 假設您在舊金山，排程在早上7:00傳送電子郵件給 **上午9:00** 傳送。 在您的智慧清單中，有下列地區的人員：

* 舊金山
* 德克薩斯州
* 紐約
* 義大利

![](assets/image2017-12-6-10-3a52-3a41.png)

紐約和義大利已經過了上午9:00，所以在這兩個時區的合格人員將會收到電子郵件，郵件依據為 **時區設定**：

* **在收件者的時區中傳遞隔天：** 各自時區的星期三上午9點， **或**

* **使用程式的預設設定時間傳遞**：星期二上午9:00 PDT （紐約 — 中午12:00 EDT和義大利 — 下午6:00 CET）。

核准程式後，它就會在15分鐘內開始執行。

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>雖然程式會啟動 _程式_ 在15分鐘內傳送電子郵件，則電子郵件不會 _已傳遞_ 就在那時。 收件者仍會根據 **時區設定** 您選擇。

## 案例2：超過25小時 {#scenario-more-than-hours}

在第二種情況下，您核准的電子郵件計畫具有 **收件者時區** 啟用且排程的傳送時間超過未來25小時。 在此情況下，程式將在中的排程時間開始執行 **最早** 世界時區(UTC + 14:00)。 全球每個時區可能有符合您智慧清單資格的人，因此從最早時區開始，我們就能在排程日期/時間將電子郵件傳送給各自時區中的所有收件者。

**開端**

現在，讓我們來談談如何 [開端](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) 搭配使用 **收件者時區**. 我們現有的「開門即用」功能要求程式至少提前12小時排程。 這對收件者時區有何意義？ 回想一下，當收件者時區啟用時，我們會在最早時區的排程時間開始執行電子郵件程式(UTC +14:00)。 因此，若要啟用 **兩者** 開頭和收件者時區，需要排程電子郵件程式 **至少比排程時間提前12小時(UTC +14:00)。**

這代表如果您位於美洲/洛杉磯，且想要同時啟用開始時間和收件者時區，則需排程方案 **34小時** 事前準備。 我們如何取得這個數字？

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

簡言之，使用收件者時區排程的電子郵件程式必須在最早時區的排程時間開始執行（亦即首先到達午夜），以符合每個時區。 因此，如果您排程電子郵件程式……

* **具有傳遞時間 _範圍_ 25小時**，程式會在15分鐘內開始執行。 已超過排程時間的收件者，將會根據您選擇的時區設定收到電子郵件。
* **具有傳遞時間 _大於_ 未來25小時**，程式會在最早的時區(UTC +14:00)的排程時間開始執行。
* **具有開頭部分**，程式會在最早時區(UTC +14:00)的排程時間前12小時開始處理。

>[!CAUTION]
>
>在您開始傳送電子郵件至實際傳送電子郵件期間取消訂閱的任何人，仍會收到電子郵件。 建議您調整取消訂閱通知，以反映取消訂閱可能需要1-2個工作日才能處理。

>[!MORELIKETHIS]
>
>* [瞭解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [電子郵件計畫的開端](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [中止傳送以收件者時區排程的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
