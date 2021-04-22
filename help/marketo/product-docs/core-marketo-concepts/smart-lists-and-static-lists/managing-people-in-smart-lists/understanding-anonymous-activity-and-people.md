---
unique-page-id: 1147322
description: 瞭解匿名活動與人員-Marketo檔案——產品檔案
title: 瞭解匿名活動與人員
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# 瞭解匿名活動和人員{#understanding-anonymous-activity-and-people}

第一次有人造訪Marketo登陸頁面（或您網站上具有[Munchkin追蹤代碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的頁面）時，Marketo會建立&#x200B;_匿名活動_，並使用瀏覽器Cookie來追蹤。 一旦識別後，就會變成人員，並合併與其瀏覽器Cookie相關的歷史記錄。

**當有** 人：

* 首次瀏覽您的Marketo登陸頁面。
* 瀏覽您網站上具有[Munchkin追蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的頁面。
* 按一下Marketo電子郵件中的「以網頁檢視」連結。[](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)

>[!NOTE]
>
>與Marketo電子郵件中的其他連結不同，[以網頁形式檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)不會以電子郵件點按方式追蹤。

當某人：

* 按一下Marketo電子郵件](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)中的[連結。
* 填寫Marketo[表單](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)。
* 使用Marketo的[SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md)或[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API（開發人員）將匿名人員與已知記錄建立關聯。

資料庫中的一個名稱可能會與許多Cookie關聯，因為人們通常使用不同的裝置和瀏覽器來瀏覽您的網站。

>[!NOTE]
>
>當匿名記錄合併到新的或現有的人員記錄中時，自訂欄位值將&#x200B;**not**&#x200B;轉移。
