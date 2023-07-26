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

Marketo有三個流程步驟可用於簡訊智慧行銷活動：

* **傳送簡訊訊息**  — 此流程動作會從Marketo智慧清單傳送訊息給訂閱使用者選取的Vibes訂閱清單的使用者。 它不會起始訂閱程式。
* **訂閱Vibes清單**  — 此流程動作會透過使用者選取的Vibes贏取行銷活動來起始簡訊訂閱程式。 然後Vibes會傳送確認訊息；收件者必須回覆該訊息，才能完成訂閱程式。
* **取消訂閱訪客清單**  — 此流程動作會從使用者選取的Vibes訂閱清單中取消訂閱每個人。

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

1. 尋找您要新增SMS流量的智慧行銷活動。 按一下 **流量** 標籤。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. 在流量上拖曳，例如： **傳送簡訊訊息**. 從下拉式清單中選取SMS訊息和Vibes清單。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >「訪客清單」選擇器可作為進一步篩選，用於篩選已在智慧清單中識別的對象，以僅鎖定屬於該「訪客」清單的潛在客戶。
   >
   >此 **訂閱Vibes清單** 和 **取消訂閱訪客清單** 流程有不同的需求。 的 **訂閱**，您必須選取Vibes清單和Vibes贏取行銷活動。 的 **取消訂閱**，則只需要變數清單。
