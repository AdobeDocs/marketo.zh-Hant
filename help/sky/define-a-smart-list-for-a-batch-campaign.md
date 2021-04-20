---
title: define-a-smart-list-for-a-batch-campaign
description: 定義批次促銷活動的智慧型清單
exl-id: 35130f40-cce5-4677-8eaf-f9d73c995ba3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# 定義批次促銷活動的智慧型清單

<br> 

智慧型清單是整個Marketo的機制，可定義要包含的「誰」（哪些人），不論是報表、清單或智慧型促銷活動。 以下是如何定義批次促銷活動的智慧清單。

1. 選擇智慧型促銷活動，然後按一下&#x200B;**[!UICONTROL Smart List]**。

   ![影像一](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. 輸入以搜尋篩選，然後拖放至畫布。 對多個濾鏡重複此步驟。

   ![影像2](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >只有篩選器的智慧型促銷活動會在「批次」模式中執行。 它會根據篩選條件在資料庫中尋找符合資格的人員，並同時透過流程執行所有篩選條件。

   >[!IMPORTANT]
   >
   >您可以新增觸發器，讓智慧型促銷活動在即時事件的基礎上，一次在一個人上執行，這會將智慧型促銷活動置於觸發器模式。

1. 按一下下拉式清單並選擇篩選運算子(例如&#x200B;**[!UICONTROL is]**、**[!UICONTROL is not]**&#x200B;等)。

   ![影像三](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >紅線表示錯誤或缺少資訊。 如果未更正，促銷活動將無效且不會執行。

1. 輸入篩選值。

   ![影像4](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>預設情況下，滿足「全部」智慧清單規則的人是
>合格。 您可以修改此項目以符合您的促銷活動需求。 如需詳細資訊，請參閱[複雜邏輯的智慧清單規則](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic)。
>
>若要一次觸發一個人的即時事件，請瞭解如何[定義智慧型促銷活動的智慧型清單 |觸發器](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger)。
