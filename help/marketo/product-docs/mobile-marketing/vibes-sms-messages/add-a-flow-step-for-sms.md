---
unique-page-id: 11379045
description: 新增SMS - Marketo檔案 — 產品檔案的流程步驟
title: 新增SMS的流程步驟
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 新增SMS的流程步驟 {#add-a-flow-step-for-sms}

Marketo有三個流程步驟，可用於您的SMS智慧行銷活動：

* **傳送SMS訊息**  — 此流操作將消息發送到訂閱用戶選擇的Vibes訂閱清單的Marketo智慧清單中的用戶。 它不會起始訂閱程式。
* **訂閱Vibes清單**  — 此流量動作會透過使用者選取的瀏覽器贏取促銷活動，起始SMS訂閱程式。 Vibes接著會傳送確認訊息；收件者必須回覆，才能完成訂閱程式。
* **取消訂閱Vibes清單**  — 此流量動作會從使用者選取的Vibes訂閱清單中取消訂閱每個人員。

>[!NOTE]
>
>傳送SMS訊息時：
>
>* Marketo用電話號碼去重複。 因此，如果多個人擁有相同的電話號碼，則只有一個人會收到這則訊息。
>* Marketo不會傳送給被列入封鎖名單或行銷暫停的人員。


有關設定流程步驟的一般資訊，請參閱 [新增流量步驟至智慧型促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

以下是使用SMS的基本概念。

1. 在「我的Marketo」中，按一下 **行銷活動**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. 尋找您要新增SMS流程的智慧行銷活動。 按一下 **流量** 標籤。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. 拖曳至流量，例如 **傳送SMS訊息**. 從下拉式清單中選取SMS訊息和視訊清單。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >「視覺效果清單」選取器可作為智慧清單中已識別之對象的進一步篩選器，以僅鎖定屬於該視覺效果清單的那些潛在客戶。
   >
   >此 **訂閱Vibes清單** 和 **取消訂閱Vibes清單** 流的要求不同。 針對 **訂閱**，您必須選取「維比斯」清單和「維比斯」贏取促銷活動。 針對 **取消訂閱**，則只需要「維比斯」清單。
