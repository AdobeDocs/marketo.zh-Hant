---
unique-page-id: 10096679
description: 範例ON24事件整合——行銷檔案——產品檔案
title: ON24事件整合範例
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---


# ON24事件整合範例 {#example-on-event-integration}

以下是ON24網路研討會的範例活動，包括促銷活動。 建立活動時，請務必先測試促銷活動，然後再執行。

## 在行銷活動中建立新事件 {#create-a-new-event-in-marketing-activities}

1. 選擇「 **新建** 」>「 **新建程式」**。

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. 選取事 **件將存在的促銷活動資料夾** 。

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. 輸入事 **件的** 「名稱」。

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. 選擇**事件**作為程 **序類型**。

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. 選擇**網路研討會**作為活動的**頻道**。

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. 按一下 **建立**。

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## 邀請（批次促銷活動）  {#invite-batch-campaign}

* **智慧型清單** -定義您要邀請誰參加活動。
* **流量**

   * 傳送電子郵件——如果這是本機資產電子郵件，則會有下列命名慣例：EventName.EmailName。 您也可以使用全域電子郵件。
   * 變更進度狀態——設為「網路研討會>已邀請」。

* **排程** -設定傳送邀請的日期。

## 註冊／確認（觸發促銷活動） {#registration-confirmation-trigger-campaign}

* **智慧型清單**

   * 根據填出表單觸 **發促銷活動**。 請務必使用「新增限制」來包含表單所在的著陸頁面 ****，尤其是當表單用於多個著陸頁面時。

>[!CAUTION]
>
>您必須使用Marketor表單來註冊活動的人員，或使用適當的API整合來註冊非Marketo表單，以將註冊資料推送至Marketo。 這對於您的活動合作夥伴整合的成功至關重要。 **注意**:如果您在非Marketo登陸頁面上使用Marketo表單，則觸發器會是 **Fills Out Form** with the Form Name。

![](assets/image2015-12-22-15-3a50-3a22.png)

* **流量**

   * **變更進展狀態** -設為網路研討會>已註冊。 **注意**:設定子促銷活動時，需要此流程步驟。 當人員的晉升狀態變更為「已注 **冊**」時，Marketo會將註冊資訊推送至ON24。

   * **傳送電子郵件** -確認電子郵件(設為「 **Operational** 」（營運），讓已註冊的未訂閱者仍可收到)。

![](assets/image2015-12-22-15-3a52-3a9.png)

**注意**:如果傳回的人員發生註冊錯誤，他們將不會收到電子郵件確認。

## 提醒（批次促銷活動） {#reminder-batch-campaign}

* **智慧清單** -使用程式 **成員進行過濾** ，並將狀態設定為「已 **註冊」**。

* **流量** -傳送電子郵件（提醒電子郵件）。

**注意**:您可以使用類似的促銷活動，傳送不 *同* 、後續的電子郵件給受邀但尚未註冊的人。

## 後續促銷活動（批次或觸發促銷活動） {#follow-up-campaign-batch-or-trigger-campaign}

* **智慧清單** -根據程式狀態的更改觸發。

![](assets/image2015-12-22-15-3a57-3a25.png)

* **流量** -傳送電子郵件。 根據計畫狀態使用選項來傳送不同的電子郵件。

![](assets/ten.png)

>[!NOTE]
>
>**相關文章**
>
>* [瞭解Marketo ON24適配器事件](understanding-marketo-on24-adapter-events.md)

>



