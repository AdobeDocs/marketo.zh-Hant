---
unique-page-id: 2952678
description: 使用傳送警報資訊權杖 {{SP_Send_Alert_Info}} - Marketo檔案 — 產品檔案
title: 使用傳送警報資訊權杖
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 使用傳送警報資訊權杖 {#use-the-send-alert-info-token-sp-send-alert-info}

此 `{{SP_Send_Alert_Info}}` Token是特殊的Token，可在建立銷售團隊的警報電子郵件時使用。

>[!TIP]
>
>此Token只有在傳送包含它的電子郵件時使用 [傳送警報](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) 流程步驟。 在「傳送電子郵件」流程步驟中使用它時無法運作。

範例警報：

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>抬頭！ 警報中的URL具有到期日，因此請確定它們具有支援這些訊息型別的步調。 到期日為 [由管理員設定](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

下列資訊包含在 `{{SP_Send_Alert_Info}}`：

* 在Marketo中將名字和姓氏作為人員詳細資料的連結
* CRM中個人的連結
* Marketo中傳送警報的行銷活動名稱
* 傳送警示的時間

>[!NOTE]
>
>只有當人員在CRM系統中（目前無法在Dynamics CRM中使用）時，CRM的連結才會出現。 Marketo和非Marketo使用者都可存取連結。

## 將SP_Send_Alert_Info權杖新增至電子郵件 {#add-the-sp-send-alert-info-token-to-an-email}

1. 選取電子郵件並按一下 **編輯草稿**.

   ![](assets/one-3.png)

1. 連按兩下您要新增Token的可編輯區域。

   ![](assets/two-3.png)

1. 將游標放在您想要Token的位置，然後按一下 **插入Token** 按鈕。

   ![](assets/three-3.png)

1. 尋找並選取 **`{{SP_Send_Alert_Info}}`** 權杖並按一下 **插入**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 按一下 **儲存**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>別忘了核准您的電子郵件。

好東西！ 此Token非常有用，您應該將其用於您為銷售團隊建立的所有警示。
