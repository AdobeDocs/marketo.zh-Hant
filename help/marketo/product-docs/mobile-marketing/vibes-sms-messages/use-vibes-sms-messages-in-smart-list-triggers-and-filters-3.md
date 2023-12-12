---
description: 在智慧清單觸發器和篩選器中使用Vibes SMS訊息 — Marketo檔案 — 產品檔案
title: 在智慧清單觸發器和篩選器中使用Vibes SMS訊息
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 6b8c54dbe95c7bc6e2f68a48de11306f3f678cb6
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 在智慧清單觸發器和篩選器中使用Vibes SMS訊息 {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

新增檔案

在您之後 [建立簡訊訊息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}，您就會想要在Smart Campaign中使用智慧列示觸發器和篩選器，以取得優點。 方法如下。

1. 在「我的Marketo」中，按一下 **行銷活動**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. 選擇您要使用簡訊資產的智慧型行銷活動。 拖曳至觸發器上方。 在此範例中，我們使用 **填寫表單**.

   ![](assets/fills-out-form-pull-over.jpg)

## 簡訊觸發程式 {#sms-triggers}

有其他可用的簡訊觸發器。 SMS觸發器僅在啟用Vibes服務時顯示。

傳送SMS訊息：

* 行銷活動>選擇新增Smart Campaign
   * 智慧清單>選擇受眾清單篩選器和正確邏輯>受眾清單：從下拉式清單（會從Vibes平台同步的行動資料庫清單）中選擇
      * 可在一個行銷活動中調整細分並利用簡訊和電子郵件篩選器及觸發器
      * Vibes篩選器：已訂閱的Vibes清單與Vibes清單的成員 — 邏輯與電子郵件一致
         * 已訂閱的Vibes清單 — 已訂閱該Vibes清單的參與者，即使他們現在已取消訂閱。   — 主要用於跨頻道行銷工作
            * 注意：未在Vibes行動資料庫清單中的取消訂閱者，將不會收到簡訊訊息
         * Vibes清單的成員 — 作用中、已確認的訂閱者
         * 新增至清單 — 此篩選器不會填入訪客清單，此篩選器適用於Marketo清單

![](assets/new-sms-search2.png)

以下是一些範例：

此 **SMS訊息退信** SMS訊息退回時，觸發器會起始流程，例如傳送電子郵件。

![](assets/sms-message-bounces-real.jpg)

此 **Vibes清單的訂閱者** 有人訂閱時，觸發器就會起始流程。

![](assets/subscribes-to-vibes-list-real.jpg)

此 **SMS訊息中的點按連結** 當有人點選SMS訊息中的連結時，觸發器就會起始流程。

![](assets/clicks-link-in-sms-message.jpg)

## 簡訊篩選器 {#sms-filters}

您也可以在智慧清單中使用視覺效果濾鏡。 此 **訂閱的視覺效果清單** 篩選器會尋找擁有下列條件的任何人： *永遠* 已訂閱影片。 這包括已取消訂閱和已刪除的人員，即使流程中省略了已刪除的人員。 此篩選器最適合用於報表。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

相較之下， **Vibes清單的成員** 篩選器尋找 _任何人_ 目前已訂閱Vibes，最適合用於智慧行銷活動或清單。

![](assets/image001.png)

>[!NOTE]
>
>所有SMS篩選器都包含 **活動日期** 預設為限制。

在智慧清單中設定Vibes觸發器和篩選器後，您可以 [定義流量](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [定義Smart Campaign的智慧清單 |觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [尋找並新增篩選器至智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
