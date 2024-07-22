---
unique-page-id: 1900573
description: 新增系統權杖作為電子郵件中的連結 — Marketo檔案 — 產品檔案
title: 新增系統權杖作為電子郵件中的連結
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# 新增系統權杖作為電子郵件中的連結 {#add-a-system-token-as-a-link-in-an-email}

您可以使用這些系統代號來自訂電子郵件中特殊連結的位置。

下列代號可在電子郵件或電子郵件範本中作為連結使用：

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>除非位於錨點連結內，否則這些Token將&#x200B;**無法**&#x200B;點選。 此外，它們&#x200B;**無法**&#x200B;內嵌到「我的Token」中。

以下說明將它們新增至電子郵件的方式：

1. 尋找並選取您的電子郵件，然後按一下&#x200B;**編輯草稿**。

   ![](assets/one-1.png)

1. 在可編輯區域中按兩下。

   ![](assets/two-1.png)

1. 反白您要轉換成具有權杖的連結的文字，然後按一下&#x200B;**插入/編輯連結**&#x200B;按鈕。

   ![](assets/three-1.png)

1. 在連結URL中輸入權杖，然後按一下&#x200B;**插入**。

   ![](assets/four-1.png)

   >[!TIP]
   >
   >複製/貼上您想要的Token： **`{{system.forwardToFriendLink}}`**、**`{{system.unsubscribeLink}}`**&#x200B;或&#x200B;**`{{system.viewAsWebpageLink}}`**

1. 按一下&#x200B;**保存**。

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>如果您使用此方法來新增「viewAsWebPageLink」系統權杖，您可以&#x200B;**不**&#x200B;使用權杖加以覆寫。 請改用[將檢視新增為網頁連結至電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)方法，此方法可讓您使用權杖覆寫「viewAsWebPageLink」。

>[!NOTE]
>
>完成時，別忘了[核准您的電子郵件](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md)。

做得很好！ 現在您知道如何將系統權杖新增為電子郵件中的連結。
