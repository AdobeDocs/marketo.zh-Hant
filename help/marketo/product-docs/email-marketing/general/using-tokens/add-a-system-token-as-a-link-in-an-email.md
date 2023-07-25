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

以下代號可用作電子郵件或電子郵件範本中的連結：

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>這些權杖將 **not** 除非位於錨點連結內，否則為可點按的。 此外，他們可以 **not** 嵌入到「我的Token」中。

以下說明如何將其新增至電子郵件：

1. 尋找並選取您的電子郵件，然後按一下 **編輯草稿**.

   ![](assets/one-1.png)

1. 在可編輯區域中連按兩下。

   ![](assets/two-1.png)

1. 反白您要轉換為具有權杖的連結的文字，然後按一下 **插入/編輯連結** 按鈕。

   ![](assets/three-1.png)

1. 在連結URL中輸入權杖並按一下 **插入**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >複製/貼上您想要的Token： **`{{system.forwardToFriendLink}}`** 或 **`{{system.unsubscribeLink}}`** 或 **`{{system.viewAsWebpageLink}}`**

1. 按一下 **儲存**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>如果您使用此方法新增「viewAsWebPageLink」系統權杖，您可以 **not** 使用Token加以覆寫。 請改用 [將檢視新增為網頁連結至電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 可讓您使用Token覆寫「viewAsWebPageLink」的方法。

>[!NOTE]
>
>別忘了 [核准您的電子郵件](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) 完成時。

幹得漂亮！ 現在您知道如何將系統權杖新增為電子郵件中的連結。
