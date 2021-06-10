---
unique-page-id: 1900573
description: 在電子郵件中新增系統代號作為連結 — Marketo檔案 — 產品檔案
title: 新增系統代號作為電子郵件中的連結
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
source-git-commit: 65caed388ac33fc9f3142102343fe43ebc186e6e
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# 在電子郵件{#add-a-system-token-as-a-link-in-an-email}中新增系統代號作為連結

您可以使用這些系統代號來自訂特殊連結在電子郵件中的位置。

下列代號可作為電子郵件或電子郵件範本中的連結：

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>除非在錨點連結內，否則這些Token將&#x200B;**不可點按**。 此外，它們也可以&#x200B;**不**&#x200B;嵌入到我的代號中。

以下說明如何將其新增至電子郵件：

1. 尋找並選取您的電子郵件，然後按一下「編輯草稿」**。**

   ![](assets/one-1.png)

1. 在可編輯區域中按兩下。

   ![](assets/two-1.png)

1. 反白顯示要轉換為具有標籤的連結的文本，然後按一下&#x200B;**插入/編輯連結**&#x200B;按鈕。

   ![](assets/three-1.png)

1. 在連結URL中輸入代號，然後按一下&#x200B;**插入**。

   ![](assets/four-1.png)

   >[!TIP]
   >
   >複製/貼上您想要的代號：**`{{system.forwardToFriendLink}}`**&#x200B;或&#x200B;**`{{system.unsubscribeLink}}`**&#x200B;或&#x200B;**`{{system.viewAsWebpageLink}}`**

1. 按一下「**儲存**」。

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>如果您使用此方法來新增「viewAsWebpageLink」系統代號，則可以&#x200B;**不**&#x200B;使用代號來覆寫它。 請改為使用[將檢視新增為網頁連結至電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)方法，讓您使用代號覆寫「viewAsWebPageLink」。

>[!NOTE]
>
>完成時，別忘了[核准您的電子郵件](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md)。

幹得好！ 現在您知道如何將系統代號新增為電子郵件中的連結。
