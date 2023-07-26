---
unique-page-id: 10098134
description: 將方案新增到參與方案流 — Marketo檔案 — 產品檔案
title: 將方案新增至參與方案流
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 將方案新增至參與方案流 {#adding-a-program-to-an-engagement-program-stream}

## 為什麼在參與方案流中使用巢狀方案？ {#why-use-a-nested-program-in-an-engagement-program-stream}

將電子郵件新增至參與計畫中的串流很容易，而且運作正常。 不過，如果您的業務需求較為複雜，將電子郵件置於計畫內或許是可行的作法。 例如，您可能想要：

* 傳送電子郵件給資料流中的子群組
* 傳送 *不同* 傳送電子郵件給串流中的子群組
* 將登陸頁面、表單或其他資產納入Nurture
* 啟用多點觸控歸因
* 新增額外流量步驟，例如警示電子郵件

## 當您在串流中使用程式時會發生什麼事？ {#what-happens-when-you-use-a-program-in-a-stream}

使用巢狀方案時，傳送電子郵件給個人的決定取決於方案會員資格和方案ID。

* 如果您不是計畫的成員，您將會收到屬於計畫的任何電子郵件一次
* 如果您是計畫的成員，您將不會收到電子郵件
* 如果您不再是會員，但先前已透過該程式收到電子郵件，您將不會收到電子郵件

當您在串流中使用程式時，您以前是否收到過該特定電子郵件並不重要。 只要電子郵件之前未寄出 *在該特定計畫中*，您可再次收到。

在參與計畫中，電子郵件和計畫可能會很棘手。 您可能會想要使用其中一個。

>[!TIP]
>
>請務必使用 **參與計畫成員** 在您的智慧清單中篩選。

## 不符合智慧清單條件的人會發生什麼事？ {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

如果有人從巢狀方案的智慧型行銷活動的智慧型清單中篩選出來，他們不會在目前轉換期間移至下一個內容片段。 他們將繼續到串流中的下一個內容片段 *關注* 轉換。

## 巢狀程式包含什麼？ {#what-does-a-nested-program-contain}

設計良好的巢狀方案包含電子郵件、報表和智慧型行銷活動。 將這些連結在一起是可行的作法。

您使用的電子郵件可以在程式、不同程式中存取，甚至在Design Studio中存取。 其存留位置將取決於您想要如何使用。

報告電子郵件位置的變更。 因此，舉例來說，如果電子郵件在Design Studio中，則電子郵件效能報表中的所有量度都會顯示在一行中 — 會合併不同的投影。 不過，在「參與資料流績效報表」中，會個別顯示不同的傳送。

>[!CAUTION]
>
>如果您想要重新傳送某些專案，最好建立新的計畫和智慧型行銷活動。

>[!MORELIKETHIS]
>
>* [將內容新增至資料流](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [瞭解計畫](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
