---
unique-page-id: 1147322
description: 瞭解匿名活動與人員——行銷檔案——產品檔案
title: 瞭解匿名活動與人員
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---


# 瞭解匿名活動與人員 {#understanding-anonymous-activity-and-people}

當有人第一次造訪Marketto [l `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) (或您網站上具有 [Munchkin追蹤代碼的頁面](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md))時，Marketo會建立*匿名*活動&#x200B;** ，並使用瀏覽器Cookie來追蹤。 一旦識別後，就會變成人員，並合併與其瀏覽器Cookie相關的歷史記錄。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

**當有人** :

* 首次造訪您的Marketing登陸頁面。

* 瀏覽您網站上具有Munchkin追蹤 [的頁面](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)。

* 按一下 [Marketo電子郵件中的「檢視為網頁](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 」連結。

>[!NOTE]
>
>與Marketo電子郵件中的其他連結不同， [「以網頁形式檢視](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 」不會以電子郵件點按方式追蹤。

當某人：

* 按一下行 [銷人員電子郵件中的連結](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)。
* 填寫行銷 [表格](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)。
* 使用Marketo的 [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846) 或 [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API（開發人員專用），將匿名人員與已知記錄建立關聯。

資料庫中的一個名稱可能會與許多Cookie關聯，因為人們通常使用不同的裝置和瀏覽器來瀏覽您的網站。

>[!NOTE]
>
>當匿名記錄合併到新的或現有的人員記錄時，自訂欄位值將 **不** 會傳輸。

