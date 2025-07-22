---
unique-page-id: 7504676
description: 瞭解期間成本 — Marketo檔案 — 產品檔案
title: 瞭解期間成本
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 瞭解期間成本 {#understanding-period-costs}

## 概觀 {#overview}

期間成本是指您在特定月份花在方案上的金額。

>[!NOTE]
>
>**範例**
>
>如果您花費$1000僱傭illustrator為將於7月啟動的[!DNL eBook]進行插圖 — [!DNL eBook]方案在7月的期間成本為$1000。
>
>如果您每月在[!DNL Google Adwords]上花費$200 - [!DNL Google Adwords]方案的期間成本為每月&#x200B;_200 $3&rbrace;。_

>[!NOTE]
>
>[瞭解程式](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[瞭解計畫成員資格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## 期間成本的計算方式 {#how-period-costs-are-calculated}

想像一下3月進行的活動，例如網路研討會。 一月份和二月份的廣告會預先招募新人。 活動後，當人們在4月和5月下載網路研討會時，也會獲得新聯絡人。

1. 將單一期間成本歸因於3月……

   ![](assets/graph1.png)

   ...之前和之後幾個月新增的連絡人將&#x200B;*僅*&#x200B;計入三月。

   ![](assets/graph2.png)

1. 將期間成本歸因於1月、2月和3月……

   ![](assets/graph3.png)

   ...僅在3月後幾個月內新增的聯絡人將計入3月。

   ![](assets/graph4.png)

1. 將期間成本歸因於1月和4月……

   ![](assets/graph5.png)

   ...在1月到3月期間新增的聯絡人將計為1月。 在4月和5月新增的聯絡人將計為4月。

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >摘要 — 沒有定義期間成本的月份將「回溯」至定義的最後一個月份。 如果沒有前期成本，則月份將「前移」到已定義的下一個月份。 如果期間成本尚未定義為&#x200B;_任何_&#x200B;個月，則程式將無法使用RCE報告。

   >[!MORELIKETHIS]
   >
   >* [在方案中使用期間成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [依期間成本篩選方案報告](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)
