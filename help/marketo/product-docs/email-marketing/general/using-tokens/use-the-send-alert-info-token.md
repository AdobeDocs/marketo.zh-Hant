---
unique-page-id: 2952678
description: 使用傳送警報資訊權杖{{SP_Send_Alert_Info}} - Marketo檔案 — 產品檔案
title: 使用傳送警報資訊權杖
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# 使用傳送警報資訊權杖 {#use-the-send-alert-info-token-sp-send-alert-info}

`{{SP_Send_Alert_Info}}` Token是特殊的Token，可在建立銷售團隊的警示電子郵件時使用。

>[!TIP]
>
>此Token只有在使用[傳送警報](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)流程步驟傳送包含它的電子郵件時，才能如預期運作。 在「傳送電子郵件」流程步驟中使用時，此功能無法運作。

範例警報：

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>抬頭！ 警示中的URL具有到期日，因此請確定它們具有支援這些訊息型別的步調。 到期日是[由管理員設定](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md)。

下列資訊包含在`{{SP_Send_Alert_Info}}`中：

* 在Marketo中將名字和姓氏作為人員詳細資料的連結
* CRM中個人的連結
* Marketo中傳送警報的行銷活動名稱
* 傳送警示的時間

>[!NOTE]
>
>只有在人員在CRM系統中（Dynamics CRM目前無法使用）時，CRM的連結才會出現。 Marketo和非Marketo使用者都可存取連結。

## 將SP_Send_Alert_Info權杖新增至電子郵件 {#add-the-sp-send-alert-info-token-to-an-email}

1. 選取電子郵件並按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/one-3.png)

1. 連按兩下您要新增權杖的可編輯區域。

   ![](assets/two-3.png)

1. 將游標置於您想要的權杖所在位置，然後按一下&#x200B;**[!UICONTROL Insert Token]**&#x200B;按鈕。

   ![](assets/three-3.png)

1. 尋找並選取&#x200B;**[!UICONTROL {{SP_Send_Alert_Info}}]** Token，然後按一下&#x200B;**[!UICONTROL Insert]**。

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>別忘了核准您的電子郵件。

好東西！ 此代號非常有用，您應該用於您為銷售團隊建立的所有警示。
