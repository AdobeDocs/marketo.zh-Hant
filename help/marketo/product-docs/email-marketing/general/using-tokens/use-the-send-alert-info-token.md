---
unique-page-id: 2952678
description: 使用傳送警報資訊Token {{SP_Send_Alert_Info}} —— 行銷人員檔案——產品檔案
title: 使用傳送警報資訊Token
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 使用傳送警報資訊Token {#use-the-send-alert-info-token-sp-send-alert-info}

`{{SP_Send_Alert_Info}}`代號是建立銷售團隊的警報電子郵件時要使用的特殊代號。

>[!TIP]
>
>此Token僅在以[傳送警報](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)流程步驟傳送包含此Token的電子郵件時如預期運作。 當用於「傳送電子郵件」流程步驟時，它將無法運作。

範例警報：   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>小心！ 警報中的URL有過期日期，因此請確定它們有支援這些類型的訊息的順序。 到期日由管理員[設定。](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md)

`{{SP_Send_Alert_Info}}`包含下列資訊：

* 名字和姓氏，作為Marketo中人員詳細資料的連結
* CRM中人員的連結
* 傳送警報之Marketo中的促銷活動名稱
* 傳送警報的時間

>[!NOTE]
>
>只有當人員在CRM系統中（目前Dynamics CRM不提供）時，才會顯示CRM的連結。 Marketo和非Marketo使用者皆可存取連結。

## 將SP_Send_Alert_Info Token添加到電子郵件{#add-the-sp-send-alert-info-token-to-an-email}

1. 選擇電子郵件，然後按一下「編輯草稿」。****

   ![](assets/one-3.png)

1. 連按兩下您要新增Token至的可編輯區域。

   ![](assets/two-3.png)

1. 將游標放在您想要標籤的位置，然後按一下「插入標籤」按鈕。****

   ![](assets/three-3.png)

1. 查找並選擇&#x200B;**`{{SP_Send_Alert_Info}}`**&#x200B;標籤，然後按一下&#x200B;**插入**。

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 按一下&#x200B;**保存**。

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**提醒**
>
>別忘了核准您的電子郵件。

好東西！ 此Token非常有用，您應將它用於您為銷售團隊建立的所有警報。