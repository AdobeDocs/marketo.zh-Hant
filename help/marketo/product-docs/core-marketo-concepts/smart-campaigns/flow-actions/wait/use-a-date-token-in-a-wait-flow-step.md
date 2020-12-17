---
unique-page-id: 1146997
description: 在等待流程步驟中使用日期Token —— 行銷人員檔案——產品檔案
title: 在等待流程步驟中使用日期Token
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# 在等待流程步驟{#use-a-date-token-in-a-wait-flow-step}中使用日期Token

您可以使用「等待流程」步驟，暫停個人在智慧型促銷活動中的歷程，直到使用日期代號的特定日期為止。 您也可以修改結束日期，以天數為單位。

>[!NOTE]
>
>這僅適用於觸發促銷活動。 您無法在批次促銷活動中使用此功能。

1. 在您的智慧型促銷活動&#x200B;**流量**&#x200B;標籤中，拖曳至&#x200B;**等待**&#x200B;流量步驟。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 按一下右側的齒輪表徵圖。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 從&#x200B;**Type**&#x200B;下拉式清單中，選擇&#x200B;**日期Token**。

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
   >您也可以使用`{{lead.`或`{{company.`代表整數欄位的Token，或`{{my.`數字類型的Token來指定天數。

1. 按一下「儲存」。

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!NOTE]
   >
   >**相關文章**
   >
   >* [在等待流程步驟中使用持續時間](use-a-duration-in-a-wait-flow-step.md)
   >* [在等待流程步驟中使用特定日期](use-a-specific-date-in-a-wait-flow-step.md)


