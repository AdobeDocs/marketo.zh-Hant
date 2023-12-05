---
description: 新增簡訊的流程步驟 — Marketo檔案 — 產品檔案
title: 新增簡訊的流程步驟
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 新增簡訊的流程步驟 {#add-a-flow-step-for-sms}

Marketo Engage有三個流程步驟可用於簡訊智慧行銷活動：

* **傳送簡訊訊息**  — 此流程動作會從Marketo智慧清單傳送訊息給訂閱使用者選擇加入Vibes訂閱清單的人員。 它不會起始訂閱程式。
* **訂閱Vibes清單**  — 此流程動作會透過使用者選取的Vibes贏取行銷活動來起始簡訊訂閱程式。 Vibes接著會傳送確認訊息；收件者必須回覆「Y」才能在24小時內確認選擇加入。 使用者選擇加入後，就會成為您相關Vibes訂閱清單的成員。
* **取消訂閱訪客清單**  — 此流量動作會從使用者選擇加入的Vibes訂閱清單中取消訂閱每個人。 當使用者對您的程式碼發文「停止」時，其人員記錄會更新，以反映他們不再是Vibes訂閱清單的成員。

>[!NOTE]
>
>傳送簡訊時：
>
>* Marketo依電話號碼進行重複資料刪除。 因此，如果多人擁有相同的電話號碼，則只有一人會收到訊息，前提是他們只有一個Vibes訂閱清單的成員。 去重複化是在Vibes訂閱清單層級，而非Marketo方案層級完成。
>* Marketo不會傳送給已加入封鎖名單或行銷遭暫停的人。

如需設定流程步驟的一般資訊，請參閱 [將流量步驟新增至Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

以下是使用SMS的基本知識。

1. 在「我的Marketo」中，按一下 **行銷活動**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. 尋找並選取您要新增SMS流程的智慧行銷活動。

   熒幕擷圖

1. 在「智慧列示」索引標籤中，選擇所需的觸發器（例如「填寫的表單」）。

   熒幕擷圖

1. 在 **流量** 標籤，在流程步驟上拖曳(例如， **傳送簡訊訊息**)。 從下拉式清單中選取SMS訊息和Vibes清單。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >「訪客清單」選擇器可作為進一步篩選，用於篩選已在智慧清單中識別的對象，以僅鎖定屬於該「訪客」清單的潛在客戶。
   >
   >此 **訂閱Vibes清單** 和 **取消訂閱訪客清單** 流程有不同的需求。 的 **訂閱**，您必須選取Vibes清單和Vibes贏取行銷活動。 的 **取消訂閱**，則只需要變數清單。
