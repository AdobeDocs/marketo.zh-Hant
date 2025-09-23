---
unique-page-id: 1147322
description: 瞭解匿名活動與人員 — Marketo檔案 — 產品檔案
title: 了解匿名活動和人員
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 3%

---

# 了解匿名活動和人員 {#understanding-anonymous-activity-and-people}

第一次有人造訪Marketo登陸頁面(或您的網站上具有[Munchkin追蹤代碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}的頁面)時，Marketo會建立&#x200B;*匿名活動*&#x200B;並使用瀏覽器Cookie進行追蹤。 在識別之後，它會變成人員，而且與其瀏覽器Cookie相關的歷史記錄會合併到。

>[!IMPORTANT]
>
>在已知&#x200B;**[!DNL Munchkin]上啟用Beta功能** V2匿名重播活動，可確保在匿名潛在客戶成功合併至已知記錄後，由匿名潛在客戶促銷活動觸發的行銷活動將一律重播。 因此，在任何重播的行銷活動中，由變更資料值步驟變更的自訂欄位將保留在已知記錄中。

**在下列情況下會建立匿名**&#x200B;活動：

* 首次造訪您的Marketo登陸頁面。
* 瀏覽網站上具有[Munchkin追蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}的頁面。
* 按一下Marketo電子郵件中的[以網頁形式檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}連結。

>[!NOTE]
>
>與Marketo電子郵件中的其他連結不同，[以網頁檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}不會被追蹤為電子郵件點選。

在下列情況下，匿名活動會合併至新的或現有人員：

* 按一下Marketo電子郵件[中的](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}連結。
* 填寫Marketo [表單](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}。
* 使用Marketo的[SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"}或[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} API （適用於開發人員），將匿名人員與已知記錄建立關聯。

資料庫中的一個名稱可能與許多Cookie繫結，因為人們經常使用不同的裝置和瀏覽器來造訪您的網站。

>[!NOTE]
>
>將匿名記錄合併至新的或現有的人員記錄時，自訂欄位值將&#x200B;*不會*&#x200B;移轉。
