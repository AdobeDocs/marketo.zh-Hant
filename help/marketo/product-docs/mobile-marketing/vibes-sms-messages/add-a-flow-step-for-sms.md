---
unique-page-id: 11379045
description: 新增簡訊的流程步驟 — Marketo檔案 — 產品檔案
title: 新增簡訊的流程步驟
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 新增簡訊的流程步驟 {#add-a-flow-step-for-sms}

Marketo有三個流程步驟，您可以在SMS智慧行銷活動中使用：

* **傳送SMS訊息**  — 此流程動作會從Marketo智慧清單傳送訊息給訂閱使用者選取的Vibes訂閱清單的使用者。 它不會起始訂閱程式。
* **訂閱Vibes清單**  — 此流程動作會透過使用者選取的Vibes贏取促銷活動來啟動簡訊訂閱程式。 然後Vibes會傳送確認訊息；收件者必須回覆該訊息才能完成訂閱程式。
* **取消訂閱Vibes清單**  — 此流程動作會從使用者選取的Vibes訂閱清單中取消訂閱每個人。

>[!NOTE]
>
>傳送簡訊時：
>
>* Marketo依電話號碼進行重複資料刪除。 因此，如果多人擁有相同的電話號碼，則只有一人會收到訊息。
>* Marketo不會傳送給已加入封鎖名單或行銷遭暫停的人。

如需設定流程步驟的一般資訊，請參閱 [將流量步驟新增至Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

以下是使用SMS的基本知識。

1. 在「我的Marketo」中，按一下 **行銷活動**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. 尋找您要新增簡訊流量的智慧行銷活動。 按一下 **流量** 標籤。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. 在流程上拖曳，例如， **傳送SMS訊息**. 從下拉式清單中選取SMS訊息和Vibes清單。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Vibes List選擇器可作為智慧清單中已識別對象的進一步篩選，以僅定位屬於該Vibes清單的潛在客戶。
   >
   >此 **訂閱Vibes清單** 和 **取消訂閱Vibes清單** 流程有不同的需求。 對象 **訂閱**，您必須選取Vibes清單和Vibes贏取促銷活動。 對象 **取消訂閱**，只需震動清單。
