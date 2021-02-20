---
unique-page-id: 11379045
description: 新增SMS —— 行銷檔案——產品檔案的流程步驟
title: 新增簡訊的流程步驟
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 新增SMS {#add-a-flow-step-for-sms}的流量步驟

Marketo有三個流程步驟，您可在SMS智慧型促銷活動中使用：

* **傳送SMS訊息** -此流量動作會傳送訊息給訂閱使用者選擇之Vibes訂閱清單之Marketo智慧型清單的使用者。它不會啟動訂閱程式。
* **訂閱檢視器清單** -此流量動作會透過使用者選取的檢視器贏取促銷活動啟動SMS訂閱程式。Vibes會傳送確認訊息；收件者必須回覆才能完成訂閱程式。
* **取消訂閱Vibes清單** -此流量動作會取消訂閱使用者選取的Vibes訂閱清單中的每個人。

>[!NOTE]
>
>傳送SMS訊息時：
>
>* Marketo透過電話號碼去重複資料。 因此，如果多人擁有相同的電話號碼，則只有一人會收到訊息。
>* Marketo不會傳送給被封鎖或暫停行銷的人員。


如需有關設定流程步驟的一般資訊，請參閱[新增流程步驟至智慧型促銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)。

以下是使用SMS的基本功能。

1. 在「我的行銷人員」中，按一下「行銷活動」**。**

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. 尋找您要新增SMS流量的智慧型促銷活動。 按一下&#x200B;**流**&#x200B;頁籤。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. 拖曳至流程上，例如&#x200B;**傳送SMS訊息**。 從下拉式清單中選取「SMS訊息」和「訪客」清單。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >「訪客清單」選擇器會對智慧型清單中已識別的對象做進一步的篩選，以僅定位屬於該「訪客」清單的訪客。
   >
   >**訂閱瀏覽清單**&#x200B;和&#x200B;**取消訂閱瀏覽清單**&#x200B;流有不同的要求。 對於&#x200B;**訂閱**，您必須選擇「訪客」清單和「訪客」贏取促銷活動。 對於&#x200B;**取消訂閱**，只需要Vibes清單。
