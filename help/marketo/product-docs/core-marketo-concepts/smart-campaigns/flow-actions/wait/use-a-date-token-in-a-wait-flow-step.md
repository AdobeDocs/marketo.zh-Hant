---
unique-page-id: 1146997
description: 在等待流程步驟中使用日期Token —— 行銷人員檔案——產品檔案
title: 在等待流程步驟中使用日期Token
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 在等待流程步驟中使用日期Token {#use-a-date-token-in-a-wait-flow-step}

您可以使用「等待流程」步驟，暫停個人在智慧型促銷活動中的歷程，直到使用日期代號的特定日期為止。 您也可以修改結束日期，以天數為單位。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>這僅適用於觸發促銷活動。 您無法在批次促銷活動中使用此功能。

1. 在智慧型促銷活 **動** 「流量」標籤中，拖曳 **至「等待流** 量」步驟。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 按一下右側的齒輪表徵圖。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 從「類 **型** 」下拉式清單中，選 **取「日期Token」**。

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. 選擇日期代號以指定等待步驟應於何時結束：

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. 若要等到目前或下一個日曆年發生日期的下一週年，請核取方塊。

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >在日期預付碼上使用此選項，可參照過去的日期，例如生日或合約開始日期。

1. （可選）您可以按指定天數修改終止日期。

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >您也可以使用代表整數欄位或 `{{lead.` 數字 `{{company.` 類型之Token來指定 `{{my.` 天數。

1. 按一下「儲存」。

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!NOTE]
   >
   >**相關文章**
   >
   >* [在等待流程步驟中使用持續時間](use-a-duration-in-a-wait-flow-step.md)
   >* [在等待流程步驟中使用特定日期](use-a-specific-date-in-a-wait-flow-step.md)


