---
unique-page-id: 7504676
description: 瞭解期間成本 — Marketo檔案 — 產品檔案
title: 瞭解期間成本
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 瞭解期間成本 {#understanding-period-costs}

## 概觀 {#overview}

期間成本是指您在特定月份花在方案上的金額。

>[!NOTE]
>
>**範例**
>
>如果您花$1000僱一名插圖師，為在7月推出的電子書做插圖，則電子書計畫在7月的期間成本將為$1000。
>
>如果您每月在Google Adwords上花費$200 - Google Adwords計畫的期間成本為$200 **每月**.

>[!NOTE]
>
>[瞭解計畫](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[瞭解計畫成員資格](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## 期間成本的計算方式 {#how-period-costs-are-calculated}

想像一下發生在三月的事件，例如網路研討會。 1月和2月的廣告會預先招募新人。 活動結束後，當人們在4月和5月下載網路研討會時，也會獲得新聯絡人。

1. 將單一期間成本歸因於3月……

   ![](assets/graph1.png)

   ...之前和之後幾個月新增的聯絡人將 *僅限* 數到3月。

   ![](assets/graph2.png)

1. 將期間成本歸因於1月、2月和3月……

   ![](assets/graph3.png)

   ...只有在3月之後幾個月才新增的聯絡人將計為3月。

   ![](assets/graph4.png)

1. 將期間成本歸因於1月和4月……

   ![](assets/graph5.png)

   ...1月到3月期間新增的聯絡人將計為1月。 在4月和5月新增的聯絡人將計為4月。

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >摘要 — 沒有已定義期間成本的月份將「迴轉」至已定義的最後一個期間。 如果沒有前期成本，月份將「前轉」到已定義的下一個月份。 如果尚未定義期間成本 _任何_ 月數，RCE中的報表不適用於該計畫。

   >[!MORELIKETHIS]
   >
   >* [在程式中使用期間成本](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [依期間成本篩選方案報表](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)
