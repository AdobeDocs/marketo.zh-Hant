---
unique-page-id: 2359504
description: 使用「寄件者地址」A/B測試 — Marketo檔案 — 產品檔案
title: 使用「寄件者地址」A/B測試
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# 使用「寄件者地址」A/B測試 {#use-from-address-a-b-testing}

您可以輕鬆地A/B測試您的電子郵件。 一項有趣的測試是 **寄件者地址** 測試。 以下說明設定方法。

>[!PREREQUISITES]
>
>[新增A/B測試](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在 **電子郵件** 圖磚，在選取電子郵件後，按一下 **新增A/B測試**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. 隨即開啟新視窗，選取 **寄件者地址** 的 **測試型別**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. 如果您有先前的測試資訊（例如主旨測試），您可以安全地按一下 **重設測試**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. 輸入第二個 **寄件者地址** 您要測試的資訊。

   >[!NOTE]
   >
   >選擇A會預先填入所選電子郵件中包含的資訊。

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >您可以按一下 **+** 以新增任意數目的寄件者地址。

1. 使用滑桿來選取您要在A/B測試中顯示的對象百分比，然後按一下 **下一個**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >不同的變化將傳送至所選測試樣本大小的相等部分。

   >[!CAUTION]
   >
   >**建議您避免將樣本大小設為100%**. 如果您使用靜態清單，將樣本大小設為100%會傳送電子郵件給對象中的每個人，而獲勝者不會獲得任何人。 如果您使用 **智慧** 清單，將樣本大小設為100%會傳送電子郵件給對象中的每個人 _當時_. 稍後當電子郵件程式再次執行時，符合智慧清單資格的任何新使用者也將收到電子郵件，因為他們現在包含在對象中。

   好的，我們快完成了。 現在我們需要 [定義A/B測試獲勝者條件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
