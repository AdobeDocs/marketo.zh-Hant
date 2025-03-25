---
unique-page-id: 1900589
description: 將追蹤連結新增至文字電子郵件 — Marketo檔案 — 產品檔案
title: 將追蹤連結新增至文字電子郵件
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
source-git-commit: b3bc6a7ec14a513e4b294852d066f9e3d0f74ef8
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# 將追蹤連結新增至文字電子郵件 {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [建立僅限文字的電子郵件](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [編輯電子郵件中的元素](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

可在Marketo中追蹤文字電子郵件連結。 讓我們看看它是如何運作的。

1. 選取您的電子郵件並按一下&#x200B;**編輯草稿**。

![](assets/one-9.png)

1. 連按兩下您要新增連結的可編輯區域。

   ![](assets/two-8.png)

1. 輸入帶有雙方括弧的URL，如下所示： `[[www.domain.com/path/page.html]]`。

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >如果在365天前&#x200B;**且**&#x200B;沒有任何人在過去180天內點按其任何連結，Marketo Engage會從我們的資料庫中刪減指向URL的路由，進而導致連結中斷。 如果您需要永久性連結，請勿使用追蹤。

1. 關閉編輯器，別忘了核准草稿。

   ![](assets/four-6.png)

>[!NOTE]
>
>mktNoTok類別功能無法與文字電子郵件中的可追蹤連結搭配使用。 僅適用於HTML電子郵件。
