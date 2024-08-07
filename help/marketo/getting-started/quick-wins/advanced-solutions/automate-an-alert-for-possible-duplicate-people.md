---
unique-page-id: 7513680
description: 針對可能的重複人員自動傳送警報 — Marketo檔案 — 產品檔案
title: 針對可能的重複人員自動傳送警報
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 針對可能的重複人員自動傳送警報 {#automate-an-alert-for-possible-duplicate-people}

想要在每次建立可能的重複人員時都顯示警示嗎？ 以下說明如何設定Smart Campaign來執行。

1. [建立新的Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}。 定義下列智慧清單：

* 觸發器： **[!UICONTROL 人員已建立]**
* 篩選器： **[!UICONTROL 重複的欄位]**。 欄位名稱&#x200B;**[!UICONTROL 是] [!UICONTROL 完整名稱]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >發揮創意。 實驗不同的欄位，以獲得更好的篩選結果。

1. 在流程步驟中，選擇[[!UICONTROL 傳送警示]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"}流程動作。

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >使用[傳送警示資訊Token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}，在您的CRM中加入此人的連結。

   >[!CAUTION]
   >
   >如果您匯入大型清單，可能會一次收到一棧這類警報！
   >
   >此外，兩個同名人員不會自動錶示他們是同一個人。

1. 在&#x200B;**[!UICONTROL 排程]**&#x200B;索引標籤中啟動行銷活動。

   ![](assets/automate-an-alert-3.png)

完成了！ 每次在Marketo中建立具有現有全名的新人員時，都會觸發此智慧型行銷活動。

>[!MORELIKETHIS]
>
>[尋找並合併重複人員](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
