---
unique-page-id: 12982903
description: 使用收件者時區排程電子郵件計畫 — Marketo檔案 — 產品檔案
title: 根據收件者時區安排電子郵件方案的時間
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 1%

---

# 根據收件者時區安排電子郵件方案的時間 {#schedule-email-programs-with-recipient-time-zone}

在啟用收件者時區的情況下，排程電子郵件程式時有兩種可能的情況：

1. 正在排程程在接下來的25小時內執行&#x200B;****
1. 正在排程程將來&#x200B;**超過**&#x200B;個25小時執行的程式（亦即下週）

## 案例1:25小時內 {#scenario-within-hours}

假設您核准已啟用收件者時區且未來25小時內已排程傳送時間的電子郵件方案。 您的智慧清單中可能會有住在已過排程時間的時區的人員。

在此案例中，我們可讓您決定如何處理此合格人員子集。 按一下電子郵件程式&#x200B;**[!UICONTROL Recipient Time Zone]**&#x200B;方塊中&#x200B;**[!UICONTROL Schedule]**&#x200B;旁的齒輪圖示。

![](assets/image2017-12-5-10-3a46-3a42.png)

這為您提供兩個選項：

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**定義**
>
>* **[!UICONTROL Deliver the following day in the recipient's time zone]**：如果電子郵件排定在星期二的9:00am發出，則已超過排定時間的時區的合格人員將在&#x200B;*星期三*&#x200B;的9:00am收到電子郵件。
>
>* **[!UICONTROL Deliver using the program's default set time]**：如果電子郵件排定在星期二9:00am發出，則已超過排定時間的時區的合格人員將會根據您的訂閱時區設定&#x200B;*收到電子郵件*。 因此，如果您的[訂閱時區設定](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md)設為PDT America/Los Angeles，這些收件者仍會在星期二的9:00am PDT收到電子郵件（無論時間是在他們自己的時區）。

>[!NOTE]
>
>[深入瞭解](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone)Marketo如何計算收件者的時區。

讓我們更詳細地考慮此情境。 假設您住在舊金山，排程於7:00am傳送電子郵件給&#x200B;**9:00am**。 您的智慧清單中有來自下列區域的人員：

* 舊金山
* 德克薩斯州
* 紐約
* 義大利

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00am已在紐約和義大利通過，因此這兩個時區的合格人員會根據&#x200B;**時區設定**&#x200B;接收電子郵件：

* **[!UICONTROL Deliver the following day in the recipient's time zone]：**&#x200B;星期三的9:00am （在各自的時區，**或**）

* **[!UICONTROL Deliver using the program's default set time]**：星期二的9:00am PDT （紐約 — 12:00pm EDT和義大利 — 6:00pm CET）。

核准程式後，它就會在15分鐘內開始執行。

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>雖然程式會在15分鐘內開始傳送電子郵件的&#x200B;*程式*，但此時不會傳送&#x200B;*封電子郵件*。 收件者仍會根據您選擇的&#x200B;**[!UICONTROL Time Zone Settings]**&#x200B;收到電子郵件。

## 案例2：超過25小時 {#scenario-more-than-hours}

在此第二個案例中，您核准已啟用&#x200B;**[!UICONTROL Recipient Time Zone]**&#x200B;且排程傳送時間超過未來25小時的電子郵件方案。 在此情況下，程式會在全球&#x200B;**最早**&#x200B;時區的排程時間開始執行(UTC + 14:00)。 全球每個時區都可能有符合您智慧清單資格的人，因此從最早的時區開始，我們就能在排定的日期/時間將電子郵件傳送給各自時區中的所有收件者。

**開始時間**

現在，讓我們討論[[!UICONTROL Head Start]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)如何搭配&#x200B;**[!UICONTROL Recipient Time Zone]**&#x200B;使用。 我們現有的「開門即用」功能要求程式至少提前12小時排程。 這對收件者時區有何意義？ 回想一下，當收件者時區啟用時，我們會在最早時區的排程時間開始執行電子郵件程式(UTC +14:00)。 因此，若要啟用&#x200B;**同時**&#x200B;開始時間和收件者時區，電子郵件程式必須排程在UTC +14 **的排程時間之前:00至少12小時。**

這表示如果您在美洲/洛杉磯，並且想要同時啟用開頭和收件者時區，您需要提前&#x200B;**34小時**&#x200B;排程程程式。 我們如何取得這個號碼？

![](assets/image2017-12-5-13-3a11-3a38.png)

<br>

簡言之，使用收件者時區排程的電子郵件程式必須在最早時區的排程時間開始執行（亦即到達午夜前），以因應每個時區。 因此，如果您排程電子郵件程式……

* **傳送時間為&#x200B;*在* 25小時內**，程式會在15分鐘內開始執行。 已超過排程時間的收件者會根據您選擇的時區設定收到電子郵件。
* **傳送時間為&#x200B;*超過* 25小時的未來**，程式將在最早時區的排程時間開始執行(UTC +14:00)。
* **如果是Head Start**，程式會在最早時區(UTC +14:00)的排程時間前12小時開始處理。

>[!CAUTION]
>
>在您開始傳送電子郵件至實際傳送電子郵件期間取消訂閱的任何人，仍會收到電子郵件。 我們建議您調整取消訂閱通知，以說明取消訂閱可能需要1-2個工作日才能處理。

>[!MORELIKETHIS]
>
>* [瞭解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* 電子郵件程式[開始使用](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [中止傳送排程為收件者時區的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
