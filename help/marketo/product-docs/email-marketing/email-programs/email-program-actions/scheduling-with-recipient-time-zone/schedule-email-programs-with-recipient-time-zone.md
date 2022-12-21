---
unique-page-id: 12982903
description: 排程電子郵件方案與收件者時區 — Marketo檔案 — 產品檔案
title: 使用收件者時區排程電子郵件方案
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# 使用收件者時區排程電子郵件方案 {#schedule-email-programs-with-recipient-time-zone}

在啟用收件者時區時，排程電子郵件程式有兩種可能的情況：

1. 計畫程式以運行 **with** 接下來的25小時
1. 計畫程式以運行 **更多** 未來超過25小時（即下週）

## 方案1:25小時內 {#scenario-within-hours}

假設您核准了已啟用「收件者時區」且已排程在未來25小時內傳送的電子郵件方案。 您的智慧清單中可能會有人居住在已排程時間經過的時區。

在此案例中，我們可讓您決定如何處理這組合格人員的子集。 按一下旁邊的齒輪圖示 **收件者時區** 在 **排程** 電子郵件程式的方塊。

![](assets/image2017-12-5-10-3a46-3a42.png)

這可提供兩個選項：

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**定義**
>
>* **在收件者的時區中傳送第二天**:如果排程在星期二上午9:00傳出電子郵件，則居住在已經過排程時間之時區的合格人員，將會收到電子郵件 *星期三* 早上9點。
>
>* **使用方案的預設設定時間傳送**:如果排程在星期二上午9:00傳出電子郵件，則居住在已經過排程時間之時區的合格人員將收到電子郵件 _根據您的訂閱時區設定_. 如果你 [訂閱時區設定](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) 設為PDT America/Los Angeles時，這些收件者仍會在星期二上午9:00（無論其所在時區的時間為何）收到電子郵件。


>[!NOTE]
>
>[深入了解](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) 關於Marketo如何計算收件者的時區。

讓我們更詳細地考慮這種情況。 假設你在舊金山，早上7:00發郵件 **上午9:00** 傳送。 在您的智慧清單中，會有來自下列地區的人員：

* 舊金山
* 德克薩斯
* 紐約
* 義大利

![](assets/image2017-12-6-10-3a52-3a41.png)

早上9:00已在紐約和義大利過去，因此這兩個時區的合格人員將會根據 **時區設定**:

* **在收件者的時區中傳送下一天：** 週三早上9點，在各自的時區， **或**

* **使用方案的預設設定時間傳送**:星期二上午9:00（紐約 — 美國東部夏令時間中午12:00，義大利 — 歐洲中部時間下午6:00）。

核准方案後，15分鐘內就會開始執行。

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>儘管計畫將啟動 _過程_ 15分鐘內傳送電子郵件時，電子郵件將不會 _傳遞_ 當時。 收件者仍會收到以 **時區設定** 你選。

## 方案2:超過25小時 {#scenario-more-than-hours}

在第二個案例中，您核准的電子郵件方案 **收件者時區** 已啟用，且排程的傳送時間未來超過25小時。 在此情況下，程式會在 **最早** 世界時區(UTC + 14:00)。 全球的每個時區都可能有符合您智慧清單資格的人員，因此，從最早的時區開始，我們便可以在排程的日期/時間將電子郵件傳送給其各自時區的所有收件者。

**開始**

現在，讓我們談談 [開始](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) 搭配 **收件者時區**. 我們現有的「搶先」功能要求該計畫至少提前12小時安排。 那麼，這對收件者時區有何意義？ 回想一下，啟用「收件者時區」後，我們會在最早時區的排程時間(UTC +14:00)開始執行電子郵件程式。 所以，為了 **both** 頭開始和收件者時區，需要排程電子郵件程式 **比預定時間(UTC +14:00)至少提前12小時。**

這表示，如果您在美國/洛杉磯，且想同時啟用「搶先」和「收件者時區」，則需要排程方案 **34小時** 事先。 我們怎麼得到這個號碼的？

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

簡而言之，與收件者時區一起排程的電子郵件程式，必須在最早時區（即最早到達午夜的時區）的排程時間開始執行，以便適應每個時區。 所以，如果你排程電子郵件程式……

* **具有傳送時間 _with_ 25小時**，程式會在15分鐘內開始執行。 已超過排程時間的收件者將根據您選擇的時區設定，收到電子郵件。
* **具有傳送時間 _大於_ 未來25小時**，程式會在最早時區的排程時間開始執行(UTC +14:00)。
* **開頭**，程式會在最早時區的排程時間前12小時開始處理(UTC +14:00)。

>[!CAUTION]
>
>如果您在開始傳送電子郵件的時間和實際傳送電子郵件的時間之間取消訂閱，仍會收到電子郵件。 建議您調整取消訂閱通知，以反映取消訂閱可能需要1至2個工作天的時間才能處理。

>[!MORELIKETHIS]
>
>* [了解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [電子郵件計畫搶灘](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [中止傳送與收件者時區排程的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

