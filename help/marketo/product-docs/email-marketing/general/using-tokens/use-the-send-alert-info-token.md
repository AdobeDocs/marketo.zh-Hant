---
unique-page-id: 2952678
description: 使用傳送警報資訊Token {{SP_Send_Alert_Info}} —— 行銷人員檔案——產品檔案
title: 使用傳送警報資訊Token
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---


# 使用傳送警報資訊Token {#use-the-send-alert-info-token-sp-send-alert-info}

代號 `{{SP_Send_Alert_Info}}` 是特殊代號，用於建立銷售團隊的警報電子郵件。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!TIP]
>
>此Token僅在以傳送警報流程步驟傳送包含此Token的電子郵件時 [如預期](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) 運作。 當用於「傳送電子郵件」流程步驟時，它將無法運作。

範例警報：   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>小心！ 警報中的URL有過期日期，因此請確定它們有支援這些類型的訊息的順序。 到期日由管 [理員設定](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md)。

下列資訊包含在 `{{SP_Send_Alert_Info}}`:

* 名字和姓氏，作為Marketo中人員詳細資料的連結
* CRM中人員的連結
* 傳送警報之Marketo中的促銷活動名稱
* 傳送警報的時間

>[!NOTE]
>
>只有當人員在CRM系統中（目前Dynamics CRM不提供）時，才會顯示CRM的連結。 Marketo和非Marketo使用者皆可存取連結。

## 將SP_Send_Alert_Info Token添加到電子郵件中 {#add-the-sp-send-alert-info-token-to-an-email}

1. 選取電子郵件，然後按一下「 **編輯草稿」**。

   ![](assets/one-3.png)

1. 連按兩下您要新增Token至的可編輯區域。

   ![](assets/two-3.png)

1. 將游標放在您想要標籤的位置，然後按一下「插入 **Token** 」按鈕。

   ![](assets/three-3.png)

1. 尋找並選取代號 **`{{SP_Send_Alert_Info}}`** ，然後按一下「 **插入**」。

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 按一下 **儲存**。

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**提醒**
>
>別忘了核准您的電子郵件。

好東西！ 此Token非常有用，您應將它用於您為銷售團隊建立的所有警報。