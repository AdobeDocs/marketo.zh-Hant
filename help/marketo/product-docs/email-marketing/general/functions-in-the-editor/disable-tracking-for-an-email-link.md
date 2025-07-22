---
unique-page-id: 1900579
description: 停用電子郵件連結的追蹤 — Marketo檔案 — 產品檔案
title: 停用電子郵件連結的追蹤
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# 停用電子郵件連結的追蹤 {#disable-tracking-for-an-email-link}

有時您並不想在電子郵件中的連結上啟用&#x200B;**Marketo追蹤URL**。 當目的地頁面不支援URL引數並且可能導致連結中斷時，這項功能會很有用。

此外，如果電子郵件是在&#x200B;**且** 365天前傳送，且過去180天內沒有人點按任何連結，Marketo Engage會從資料庫中刪減指向URL的路由，進而導致連結中斷。 因此，如果您需要讓連結成為永久連結，您應停用追蹤。

1. 選取您的電子郵件並按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/one-7.png)

1. 連按兩下包含連結的可編輯區段。

   ![](assets/two-6.png)

1. 按一下有問題的連結，然後按一下&#x200B;**插入/編輯連結**&#x200B;按鈕。

   ![](assets/three-6.png)

1. 在「編輯連結」彈出式視窗中，取消勾選「**[!UICONTROL Track Link]**」核取方塊。

   ![](assets/four-4.png)

1. 您會注意到&#x200B;**[!UICONTROL Include mkt_tok]方塊**&#x200B;消失。 按一下「**[!UICONTROL Apply]**」。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >取消僅核取&#x200B;**包含mkt_tok**&#x200B;仍可追蹤連結，但在重新導向後，目的地URL將不會包含mkt_tok查詢字串引數。 Marketo登陸頁面和Munchkin會使用此引數，以確保正確追蹤人員活動（例如當人員取消訂閱電子郵件時）。 您應該避免使用此功能，除非您因引數出現而在網站上看到奇怪的行為。

1. 按一下「**[!UICONTROL Save]**」。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!CAUTION]
   >
   >若要停用電子郵件範本中連結的點選追蹤，或電子郵件的[文字版本](/help/marketo/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.md){target="_blank"}，請在字串的`mktNoTrack`開頭&#x200B;*新增*，而非結尾，如下列範例所示： `<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`。 否則，可能會導致連結消失。 如果您需要上述程式碼實作的協助，請洽詢您的網頁開發人員。
