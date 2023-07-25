---
unique-page-id: 1147322
description: 瞭解匿名活動與人員 — Marketo檔案 — 產品檔案
title: 瞭解匿名活動和人員
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 瞭解匿名活動和人員 {#understanding-anonymous-activity-and-people}

第一次有人造訪Marketo登陸頁面(或您的網站上具有 [Munchkin追蹤程式碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)，Marketo會建立 _匿名活動_ 和使用瀏覽器Cookie來追蹤。 在識別之後，它會變成一個人，而且與其瀏覽器Cookie關聯的歷史記錄會合併到中。

>[!IMPORTANT]
>
>啟用測試版功能 **已知上的Munchkin V2匿名重播活動** 可確保在匿名銷售機會成功合併至已知記錄後，由匿名銷售機會促銷活動所觸發的行銷活動將一律重播。 因此，任何重播行銷活動中，由變更資料值步驟變更的自訂欄位將保留在已知記錄中。

**匿名** 活動是在有人符合以下條件時建立：

* 首次造訪您的Marketo登陸頁面。
* 造訪您網站上具有 [Munchkin追蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* 按一下 [以網頁檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Marketo電子郵件中的連結。

>[!NOTE]
>
>不同於Marketo電子郵件中的其他連結， [以網頁檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 不會追蹤為電子郵件點選。

某人出現下列情況時，匿名活動會合併至新的或現有的人員中：

* 按一下 [Marketo電子郵件中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* 填寫Marketo [表單](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* 使用Marketo的 [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) 或 [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) （適用於開發人員）將匿名人員與已知記錄建立關聯的API。

資料庫中有一個名稱可能與許多Cookie連結，因為人們經常使用不同的裝置和瀏覽器造訪您的網站。

>[!NOTE]
>
>當匿名記錄合併到新的或現有的個人記錄中時，自訂欄位值將 **not** 移轉過去。
