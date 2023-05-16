---
unique-page-id: 7513680
description: 自動提醒可能重複的人員 — Marketo檔案 — 產品檔案
title: 自動提供可能重複人員的警報
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 615107dc9da9fec4b6d06c5ca6bc0a2c03e84fdc
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 自動提供可能重複人員的警報 {#automate-an-alert-for-possible-duplicate-people}

是否要在每次建立可能的重複人員時發出警報？ 以下說明如何設定智慧型行銷活動。

1. [建立新的智慧型行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. 定義下列智慧清單：

* 觸發： **[!UICONTROL 已建立人員]**
* 篩選： **[!UICONTROL 複製欄位]**. 欄位名稱 **[!UICONTROL is] [!UICONTROL 完整名稱]**

   ![](assets/automate-an-alert-1.png)

   >[!TIP]
   >
   >有創意。 實驗不同的場，得到更好的濾波效果。

1. 在流程步驟中，選擇 [[!UICONTROL 傳送警報]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"} 流量動作。

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >使用 [傳送警報資訊Token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} 在CRM中包含連結至人員的方式。

   >[!CAUTION]
   >
   >如果您匯入大型清單，可能會同時收到一堆警報！
   >
   >另外，兩個同名的人並不自動表示他們是同一個人。

1. 在 **[!UICONTROL 排程]** 標籤。

   ![](assets/automate-an-alert-3.png)

就這樣！ 每次在Marketo中建立現有全名的新人員時，都會觸發此智慧型促銷活動。

>[!MORELIKETHIS]
>
>[查找和合併重複人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
