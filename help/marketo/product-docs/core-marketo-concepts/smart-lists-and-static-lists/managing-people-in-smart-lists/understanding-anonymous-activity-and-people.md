---
unique-page-id: 1147322
description: 了解匿名活動與人員 — Marketo檔案 — 產品檔案
title: 了解匿名活動和人員
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
source-git-commit: cc66f4ff2e3e0e6ddfabab91215e3ad31f3b9226
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 了解匿名活動和人員 {#understanding-anonymous-activity-and-people}

第一次有人造訪Marketo登陸頁面(或您網站上具有 [Munchkin追蹤程式碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo會建立 _匿名活動_ 並使用瀏覽器Cookie來追蹤。 識別後，就會變成人員，並合併與其瀏覽器Cookie相關聯的歷史記錄。

>[!IMPORTANT]
>
>啟用測試版功能 **Munchkin V2匿名重播活動，已知** 確保匿名銷售機會促銷活動觸發的促銷活動在成功合併至已知記錄後，一律會重播。 因此，在任何重播的促銷活動中，依「變更資料值」步驟變更的自訂欄位將會保留在已知記錄中。

**匿名** 當有人：

* 首次造訪您的Marketo登陸頁面。
* 瀏覽您網站上具有 [Munchkin追蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* 按一下 [作為網頁查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Marketo電子郵件中的連結。

>[!NOTE]
>
>不同於Marketo電子郵件中的其他連結， [作為網頁查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 不會以電子郵件點按的形式追蹤。

當有人：

* 點按 [Marketo電子郵件中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* 填寫Marketo [表單](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* 使用Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) 或 [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API（供開發人員使用），將匿名人員與已知記錄建立關聯。

資料庫中的一個名稱可能與許多Cookie相關聯，因為人們經常使用不同的裝置和瀏覽器來造訪您的網站。

>[!NOTE]
>
>當匿名記錄合併到新的或現有的人員記錄時，自訂欄位值將 **not** 轉移。
