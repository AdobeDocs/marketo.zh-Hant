---
description: 在智慧清單觸發器和篩選器中使用SMS選項 — Marketo檔案 — 產品檔案
title: 在智慧清單觸發器和篩選器中使用簡訊選項
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 8e56b571a34451d6b0436dc041efaf0fd575db36
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# 在智慧清單觸發器和篩選器中使用簡訊選項 {#use-sms-options-in-smart-list-triggers-and-filters}

新增檔案

在您之後 [建立簡訊訊息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}，您就會想要在Smart Campaign中使用智慧列示觸發器和篩選器，以取得優點。

>[!PREREQUISITES]
>
>SMS觸發器/篩選器僅在以下情況下出現： [已啟用Vibes服務](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## 簡訊觸發程式 {#sms-triggers}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-1.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-2.png"></td>
  </tr>
</table>

以下是一些範例：

此 **SMS訊息退信** SMS訊息退回時，觸發器會起始流程，例如傳送電子郵件。

此 **Vibes清單的訂閱者** 有人訂閱時，觸發器就會起始流程。

此 **SMS訊息中的點按連結** 當有人點選SMS訊息中的連結時，觸發器就會起始流程。

## 簡訊篩選器 {#sms-filters}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-3.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-4.png"></td>
  </tr>
</table>

您也可以在智慧清單中使用視覺效果濾鏡。 此 **訂閱的視覺效果清單** 篩選器會尋找擁有下列條件的任何人： *永遠* 已訂閱影片。 這包括已取消訂閱和已刪除的人員，即使流程中省略了已刪除的人員。 此篩選器最適合用於報表。

相較之下， **Vibes清單的成員** 篩選器尋找 _任何人_ 目前已訂閱Vibes，最適合用於智慧行銷活動或清單。

>[!NOTE]
>
>所有SMS篩選器都包含 **活動日期** 預設為限制。

在智慧清單中設定Vibes觸發器和篩選器後，您可以 [定義流量](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [傳送簡訊訊息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [定義Smart Campaign的智慧清單 |觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [尋找並新增篩選器至智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
