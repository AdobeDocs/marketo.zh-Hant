---
description: 在Smart Campaign中使用簡訊選項 — Marketo檔案 — 產品檔案
title: 在智慧行銷活動中使用簡訊選項
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 在智慧行銷活動中使用簡訊選項 {#using-sms-options-in-a-smart-campaign}

在您[建立SMS訊息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}後，您將會想要在Smart Campaign中使用智慧清單觸發器和篩選器來取得優點。

>[!NOTE]
>
>如果您要傳送SMS訊息，我們有[特定文章](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}。

>[!PREREQUISITES]
>
>SMS觸發器/篩選器只在[Vibes服務已啟用](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}時才會出現。

## 簡訊觸發程式 {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

以下是一些範例：

**SMS訊息退回**&#x200B;觸發程式會在SMS訊息退回時啟動流程，例如傳送電子郵件。

當人員訂閱時，**Subscribes to Vibes List**&#x200B;觸發程式會起始流程。

當有人點按SMS訊息中的連結時，**點按SMS訊息中的連結**&#x200B;觸發器會起始流程。

## 簡訊篩選器 {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

**已訂閱的Vibes清單**&#x200B;篩選器會尋找任何已&#x200B;*ever*&#x200B;訂閱Vibes的人。 這包括已取消訂閱和已刪除的人員，即使流程中省略了已刪除的人員。 此篩選器最適合用於報表。

相較之下，**Vibes清單的成員**&#x200B;篩選器會找出目前訂閱了Vibes的&#x200B;_任何人_，最適合用於智慧行銷活動或清單。

>[!NOTE]
>
>所有SMS篩選器預設都包含&#x200B;**活動日期**&#x200B;限制。

## 簡訊流程步驟 {#sms-flow-steps}

有三個簡訊流程步驟可供選擇。

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>傳送簡訊訊息</b></td>
    <td>此流程動作會從Marketo智慧清單傳送訊息給訂閱使用者選擇加入的Vibes訂閱清單的使用者。 它不會起始訂閱程式。 <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">深入瞭解</a>。</td>
  </tr>

<tr>
    <td style="width:20%"><b>訂閱Vibes清單</b></td>
    <td>此流程動作會透過使用者選取的Vibes贏取行銷活動來起始簡訊訂閱程式。 然後Vibes會傳送確認訊息，收件者必須在24小時內以「Y」回覆該訊息，以確認選擇加入。 使用者選擇加入後，就會成為您相關Vibes訂閱清單的成員。</td>
  </tr>
  <tr>
    <td style="width:20%"><b>取消訂閱訪客清單</b></td>
    <td>此流量動作會從使用者選擇加入的Vibes訂閱清單中取消訂閱每個人。 當使用者將「STOP」文字傳送到您的程式碼時，其人員記錄會更新，以反映他們不再是Vibes訂閱清單的成員。</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>**訂閱Vibes清單**&#x200B;與&#x200B;**取消訂閱Vibes清單**&#x200B;流程具有不同的需求。 針對&#x200B;**訂閱**，您必須選取Vibes清單和Vibes贏取行銷活動。 對於&#x200B;**取消訂閱**，僅需要Vibes清單。

>[!MORELIKETHIS]
>
>* [傳送SMS訊息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [定義智慧行銷活動的智慧清單 | 觸發器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [定義智慧行銷活動的智慧清單 | 批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
