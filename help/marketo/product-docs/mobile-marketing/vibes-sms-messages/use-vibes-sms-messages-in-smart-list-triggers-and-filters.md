---
unique-page-id: 11378871
description: 在智慧清單觸發器和篩選器中使用Vibes SMS訊息 — Marketo檔案 — 產品檔案
title: 在智慧清單觸發器和篩選器中使用Vibes SMS訊息
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# 在智慧清單觸發器和篩選器中使用Vibes SMS訊息 {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

在您之後 [建立Vibes SMS訊息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)，您就會想要在智慧行銷活動中使用智慧清單觸發器和篩選器，以獲得好處。 方法如下。

1. 在「我的Marketo」中，按一下 **行銷活動**.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. 選擇您要使用簡訊資產的智慧型行銷活動。 拖曳到觸發程式上，例如熱門播放器 **填寫表單**.

   ![](assets/fills-out-form-pull-over.jpg)

## 簡訊觸發程式 {#sms-triggers}

有其他可用的簡訊觸發器。 SMS觸發器僅在啟用Vibes服務時顯示。

![](assets/new-sms-search2.png)

以下是一些範例：

SMS訊息退回觸發程式會起始流程，例如在SMS訊息退回時傳送電子郵件。

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
