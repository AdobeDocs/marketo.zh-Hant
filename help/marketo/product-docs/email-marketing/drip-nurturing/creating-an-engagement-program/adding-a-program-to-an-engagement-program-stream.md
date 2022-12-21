---
unique-page-id: 10098134
description: 將方案新增至參與方案串流 — Marketo檔案 — 產品檔案
title: 將方案新增至參與方案串流
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 將方案新增至參與方案串流 {#adding-a-program-to-an-engagement-program-stream}

## 為何在參與程式流中使用巢狀程式？ {#why-use-a-nested-program-in-an-engagement-program-stream}

在參與計畫中將電子郵件新增至資料流很簡單，而且運作正常。 不過，如果您的業務需求更複雜，將電子郵件放入計畫中或許有意義。 例如，您可能想要：

* 傳送電子郵件給資料流中的人員子群組
* 傳送 *不同* 發送電子郵件給資料流中的子組
* 包括登錄頁面、表單或培養內的其他資產
* 啟用多點接觸歸因
* 新增額外的流量步驟，例如警報電子郵件

## 在資料流中使用程式會發生什麼事？ {#what-happens-when-you-use-a-program-in-a-stream}

使用巢狀程式時，傳送電子郵件給人員的決定是根據程式成員資格和程式ID。

* 如果您不是計畫的成員，您將會收到屬於計畫的任何電子郵件一次
* 如果您是計畫的成員，您將不會收到電子郵件
* 如果您不再是會員，但之前已透過該方案收到電子郵件，則不會收到電子郵件

在資料流中使用程式時，如果您之前收到過該特定電子郵件並不重要。 只要之前沒有傳送電子郵件 *在*，您可以再次收到。

它可能會在參與計畫中複雜地混合電子郵件和程式。 您可能想使用其中一個。

>[!TIP]
>
>請務必使用 **參與計畫成員** 篩選。

## 不符合智慧清單條件的人會發生什麼事？ {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

如果從巢狀方案的智慧促銷活動的智慧清單中篩選出某個人，則在目前的轉換期間，他們不會繼續移至下一個內容片段。 他們會移至資料流中的下一段內容，以供 *下列* 演出。

## 嵌套程式包含什麼？ {#what-does-a-nested-program-contain}

精心設計的巢狀方案包含電子郵件、報表和智慧型行銷活動。 把這些放在一起是有道理的。

您使用的電子郵件可以在方案中、不同方案中，甚至在Design Studio中存留。 它的生存位置取決於你想如何使用它。

使用電子郵件位置回報變更。 因此，例如，如果電子郵件位於Design Studio中、電子郵件效能報表中，所有量度都會以一行顯示 — 會結合不同的轉播。 不過，在「參與資料流績效報表」中，不同的傳送會個別顯示。

>[!CAUTION]
>
>如果您想要重新傳送某個內容，最好建立新的方案和聰明的行銷活動。

>[!MORELIKETHIS]
>
>* [新增內容至資料流](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [了解方案](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

