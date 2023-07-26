---
unique-page-id: 2949716
description: 使用Outlook的電子郵件增益集傳送及追蹤電子郵件 — Marketo檔案 — 產品檔案
title: 使用Outlook的電子郵件增益集傳送及追蹤電子郵件
exl-id: 81c2ce86-1528-48ad-8848-ee5a828f9ff7
feature: Marketo Sales Insights
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 使用Outlook的電子郵件增益集傳送及追蹤電子郵件 {#send-and-track-an-email-with-the-email-add-in-for-outlook}

您可以直接從Outlook使用Marketo傳送及追蹤電子郵件。

>[!PREREQUISITES]
>
>如果尚未安裝，請安裝 [適用於Outlook的Marketo電子郵件增益集](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md).

>[!NOTE]
>
>「銷售分析動作」功能（包括「傳送銷售電子郵件」、「新增至銷售促銷活動」和「工作」）在Gmail和Outlook的「銷售分析電子郵件」外掛程式中無法使用。 目前，使用Sales Insight電子郵件外掛程式時，使用者只能從電子郵件使用者端傳送包含或不包含Marketo電子郵件範本的可追蹤電子郵件。

1. 開啟Microsoft Outlook並建立新電子郵件。

   ![](assets/image2014-9-23-16-3a6-3a46.png)

   >[!CAUTION]
   >
   >如果您在電子郵件中包含多個收件者，則會在第一個收件者底下追蹤所有活動。

1. 依照正常方式撰寫電子郵件，然後按一下 **傳送和追蹤**.

   ![](assets/image2014-9-23-16-3a7-3a1.png)

   >[!NOTE]
   >
   >如果您傳送電子郵件給不在Marketo例項中的人員，系統會自動為他們建立人員記錄。 他們的姓氏將一律為「mktUnknown」，以便您輕鬆找到。

   >[!TIP]
   >
   >如果您想使用Marketo範本，請參閱 [使用範本從Outlook傳送及追蹤](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md).

1. 檢視預覽並按一下 **傳送**.

   ![](assets/image2014-9-23-16-3a7-3a13.png)

   >[!CAUTION]
   >
   >反垃圾郵件技術通常會拒絕在傳送電子郵件後20秒內進行的開啟和點按，因此在測試時請至少等候這麼久才開啟/點按。

   若要檢視哪些人已收到透過Outlook傳送的電子郵件，請使用「已傳送銷售電子郵件」篩選條件建立智慧清單。

   ![](assets/was-sent-sales-email.png)

這太簡單了！ 即使此電子郵件是由銷售人員的Outlook傳送，仍會在Marketo中追蹤。

>[!MORELIKETHIS]
>
>[在Marketo中記錄潛在客戶寄來的傳入郵件](/help/marketo/product-docs/marketo-sales-insight/using-msi/log-inbound-mail-from-your-leads-in-marketo.md)
