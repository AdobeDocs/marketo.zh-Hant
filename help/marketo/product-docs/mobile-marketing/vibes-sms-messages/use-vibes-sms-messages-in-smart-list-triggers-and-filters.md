---
unique-page-id: 11378871
description: 在智慧清單觸發器和篩選器中使用瀏覽器SMS訊息 — Marketo檔案 — 產品檔案
title: 在智慧清單觸發器和篩選器中使用瀏覽器SMS訊息
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# 在智慧清單觸發器和篩選器中使用瀏覽器SMS訊息 {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

在 [建立瀏覽器SMS訊息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)，您會想要在智慧型行銷活動中使用智慧清單觸發器和篩選器，以獲得優點。 這是方法。

1. 在「我的Marketo」中，按一下 **行銷活動**.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. 選擇您要使用SMS資產的智慧型行銷活動。 拖曳至觸發器，例如熱門 **填寫表單**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS觸發器 {#sms-triggers}

還有其他SMS觸發器可供使用。 只有在啟用Vibes服務時，SMS觸發器才會出現。

![](assets/new-sms-search2.png)

以下是一些範例：

SMS訊息彈回觸發會起始流程，例如在SMS訊息彈回時傳送電子郵件。

![](assets/sms-message-bounces-real.jpg)

此 **維比清單訂閱** 觸發器會在人員訂閱時啟動流程。

![](assets/subscribes-to-vibes-list-real.jpg)

此 **在SMS訊息中點按連結** 觸發程式會在使用者點按SMS訊息中的連結時啟動流程。

![](assets/clicks-link-in-sms-message.jpg)

## SMS篩選器 {#sms-filters}

您也可以在智慧清單中使用維比斯篩選器。 此 **已訂閱維比清單** 篩選器查找 *ever* 已訂閱Vibes。 這包括已取消訂閱和已刪除的人員，即使流程中遺漏已刪除的人員。 此篩選器最適合用於報表。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

相反， **維布清單成員** 篩選器查找 _任何人_ 目前已訂閱Vibes，最適合用於智慧型行銷活動或清單。

![](assets/image001.png)

>[!NOTE]
>
>所有SMS篩選器都包含 **活動日期** 約束。

在您的智慧清單中設定Vibes觸發器和篩選器後，您可以 [定義流](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [定義智慧促銷活動的智慧清單 |觸發](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [尋找篩選器並新增至智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

