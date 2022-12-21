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

# 新增系統代號作為電子郵件中的連結 {#add-a-system-token-as-a-link-in-an-email}

您可以使用這些系統代號來自訂特殊連結在電子郵件中的位置。

下列代號可作為電子郵件或電子郵件範本中的連結：

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>這些代號將 **not** 除非在錨點連結內，否則可供點按。 此外，他們可以 **not** 嵌入到我的令牌中。

以下說明如何將其新增至電子郵件：

1. 尋找並選取您的電子郵件，然後按一下 **編輯草稿**.

   ![](assets/one-1.png)

1. 在可編輯區域中按兩下。

   ![](assets/two-1.png)

1. 反白顯示您要轉換為具有代號的連結，然後按一下 **插入/編輯連結** 按鈕。

   ![](assets/three-1.png)

1. 在連結URL中輸入代號，然後按一下 **插入**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >複製/貼上您想要的代號： **`{{system.forwardToFriendLink}}`** 或 **`{{system.unsubscribeLink}}`** 或 **`{{system.viewAsWebpageLink}}`**

1. 按一下 **儲存**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>如果您使用此方法來新增「viewAsWebpageLink」系統代號，您可以 **not** 使用Token覆寫。 請改用 [將檢視新增為電子郵件的網頁連結](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 可讓您使用Token覆寫「viewAsWebPageLink」的方法。

>[!NOTE]
>
>別忘了 [核准電子郵件](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) 時才能使用。

幹得好！ 現在您知道如何將系統代號新增為電子郵件中的連結。
