---
unique-page-id: 2952678
description: 使用傳送警報資訊Token {{SP_Send_Alert_Info}} - Marketo檔案 — 產品檔案
title: 使用傳送警報資訊Token
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 使用傳送警報資訊Token {#use-the-send-alert-info-token-sp-send-alert-info}

此 `{{SP_Send_Alert_Info}}` token是為您的銷售團隊建立警報電子郵件時要使用的特殊token。

>[!TIP]
>
>此代號只有在傳送包含此代號的電子郵件時，才能如預期般運作 [傳送警報](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) 流程步驟。 在「傳送電子郵件流程」步驟中使用時，將無法運作。

範例警報：

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>抬頭！ 警報中的URL有到期日，因此請確定它們有可支援這些類型的訊息的順序。 到期日為 [由管理員設定](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

下列資訊包含在 `{{SP_Send_Alert_Info}}`:

* 以名字和姓氏作為Marketo中人員詳細資料的連結
* CRM中人員的連結
* 傳送警報的Marketo中的促銷活動名稱
* 傳送警報的時間

>[!NOTE]
>
>只有當人員位於CRM系統中（目前不適用於Dynamics CRM）時，才會顯示CRM的連結。 Marketo和非Marketo使用者都可存取連結。

## 將SP_Send_Alert_Info令牌添加到電子郵件 {#add-the-sp-send-alert-info-token-to-an-email}

1. 選取電子郵件，然後按一下 **編輯草稿**.

   ![](assets/one-3.png)

1. 連按兩下您要新增代號的可編輯區域。

   ![](assets/two-3.png)

1. 將游標置於您想要的代號所在的位置，然後按一下 **插入代號** 按鈕。

   ![](assets/three-3.png)

1. 尋找並選取 **`{{SP_Send_Alert_Info}}`** 代號，按一下 **插入**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 按一下 **儲存**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>別忘了核准您的電子郵件。

好東西！ 此代號非常有用，您應將其用於您為銷售團隊建立的所有警報中。
