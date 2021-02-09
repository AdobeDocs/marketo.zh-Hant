---
unique-page-id: 12982903
description: 排程電子郵件計畫及收件者時區——行銷人員檔案——產品檔案
title: 計畫包含收件者時區的電子郵件程式
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 計畫收件者時區{#schedule-email-programs-with-recipient-time-zone}的電子郵件程式

在啟用「收件者時區」時，排程電子郵件程式時有兩種可能的情形：

1. 將程式排程為在&#x200B;**內運行**，接下來25小時
1. 將程式安排為在將來運行&#x200B;**>>**&#x200B;超過25小時（即下週）

## 方案1:25小時內{#scenario-within-hours}

假設您核准啟用「收件者時區」且排程在25小時內傳送的電子郵件方案。 您的智慧型清單中可能會有人居住在已排程時間過去的時區。

在此案例中，我們允許您決定如何處理這些合格人員子集。 按一下電子郵件程式&#x200B;**計畫**&#x200B;表徵圖中&#x200B;**收件人時區**&#x200B;旁邊的齒輪表徵圖。

![](assets/image2017-12-5-10-3a46-3a42.png)

這提供了兩個選項：

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**定義**
>
>* **在收件者的時區提供下一天**:如果電子郵件排程在星期二上午9:00外出，則居住在已排程時間經過的時區的合格人員將於週三上午9:00收到 ** 電子郵件。
   >
   >
* **使用程式的預設設定時間提供**:如果電子郵件排程在星期二上午9:00外出，則居住在已排程時間經過的時區的合格人員，會根據您的訂閱時區設定 _收到電子郵件_。因此，如果您的[訂閱時區設定](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md)設定設為PDT America/Los Angeles，這些收件者仍會在星期二上午9:00（無論其所在時區的時間為何）收到電子郵件。


>[!NOTE]
>
>[進一](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) 步瞭解Marketo如何為收件者計算時區。

讓我們更詳細地考慮這種情況。 假設您在舊金山，請在早上7:00排程電子郵件，以接收&#x200B;**9:00am**&#x200B;傳送。 在您的智慧清單中，有來自下列地區的人員：

* 舊金山
* 德克薩斯州
* 紐約
* 義大利

![](assets/image2017-12-6-10-3a52-3a41.png)

早上9:00已在紐約和義大利經過，因此這兩個時區的合格人員將會根據&#x200B;**時區設定**&#x200B;收到電子郵件：

* **在收件者的時區傳送第二天：** 星期三上午9:00（在各自的時區）, **或**

* **使用程式的預設設定時間提供**:星期二上午9:00美元（紐約東部夏令時間下午12:00，義大利東部時間下午6:00）。

一旦您核准程式後，該程式會在15分鐘內開始執行。

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>雖然程式會在15分鐘內開始傳送電子郵件的&#x200B;_程式_，但當時不會傳送&#x200B;_電子郵件。_&#x200B;收件者仍會收到您選擇的&#x200B;**時區設定**&#x200B;電子郵件。

## 方案2:超過25小時{#scenario-more-than-hours}

在第二種情況中，您核准啟用&#x200B;**收件者時區**&#x200B;且排程的傳送時間超過25小時的電子郵件程式。 在這種情況下，程式將在世界上最早&#x200B;**的**&#x200B;時區(UTC + 14:00)的預定時間開始運行。 全球每個時區都有符合您智慧型清單資格的人員，因此從最早的時區開始，我們可以在排程的日期／時間將電子郵件傳送給其各自時區的所有收件者。

**開始前行**

現在，讓我們討論[Head Start](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)如何與&#x200B;**Recipient Time Zone**&#x200B;搭配使用。 我們現有的Head Start功能要求計畫至少提前12小時完成。 那麼，這對收件者時區意味著什麼？ 請記住，啟用「收件者時區」後，我們會在最早時區(UTC +14:00)的排程時間開始執行電子郵件程式。 因此，要啟用&#x200B;**兩個**&#x200B;頭開始時區和接收者時區，電子郵件程式必須至少提前12小時（以UTC +14:00表示）計畫。****

這表示如果您在美國／洛杉磯，並想要同時啟用「開始前」和「接收者時區」，則需要事先安排計畫&#x200B;**34小時**。 我們怎麼得到這個號碼的？

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

簡而言之，使用「收件者時區」排程的電子郵件程式必須在排程的時間開始在最早的時區（亦即最早到達午夜的時區）執行，以便適應每個時區。 所以，如果您排程電子郵件程式……

* **在25小時內 _傳_ 送時間**，程式將在15分鐘內開始執行。已超過排程時間的收件者，將會根據您選擇的時區設定收到電子郵件。
* **未來的發 _送時_ 間超過25小時**，程式會在最早時區(UTC +14:00)的排程時間開始執行。
* **使用Head Start**，該程式在最早時區的預定時間前12小時開始處理(UTC +14:00)。

>[!CAUTION]
>
>在您開始傳送電子郵件至實際傳送電子郵件之間取消訂閱的人，仍會收到電子郵件。 我們建議您調整取消訂閱通知，以反映取消訂閱可能需要1-2個工作天才能處理。

>[!MORELIKETHIS]
>
>* [瞭解收件者時區](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [電子郵件計畫快速入門](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [中止傳送以收件者時區排程的電子郵件程式](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

