---
unique-page-id: 2359520
description: 使用「日期/時間」A/B測試 — Marketo檔案 — 產品檔案
title: 使用「日期/時間」A/B測試
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 使用「日期/時間」A/B測試 {#use-date-time-a-b-testing}

您可以輕鬆A/B測試您的電子郵件。 一個測試是 **日期/時間** 測試。 這會測試在某天或一週中的某天何時最適合傳送電子郵件。 下面是如何設定它。

>[!PREREQUISITES]
>
>[新增A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在 **電子郵件** 拼貼，按一下 **新增A/B測試**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. 新視窗隨即開啟。 選擇 **日期/時間** for **測試類型**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. 如果您有先前的測試資訊（如主題測試），您可以安全地按一下 **重置測試**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. 選取您的首次日期/時間的日期。

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. 選取您的首次日期/時間。

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. 對您的第二個日期/時間也一樣。

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. 使用滑桿來選擇您要在A/B測試中佔受眾的百分比，然後按一下 **下一個**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >不同的變化將應用於所選測試樣本大小的相等部分。

   >[!CAUTION]
   >
   >**建議您避免將樣本大小設為100%**. 如果您使用靜態清單，將樣本大小設為100%會傳送電子郵件給對象中的所有人，而獲勝者不會收到任何人。 如果您使用 **智慧** 清單中，將樣本大小設為100%會傳送電子郵件給對象中的所有人 _當時_. 當電子郵件程式在稍後日期再次執行時，符合智慧清單資格的任何新人員也會收到電子郵件，因為他們現在已包含在對象中。

   好，我們再近一步。 現在我們需要 [定義A/B測試獲勝者條件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
