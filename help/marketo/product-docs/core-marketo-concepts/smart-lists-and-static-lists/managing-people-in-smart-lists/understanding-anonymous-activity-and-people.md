---
unique-page-id: 1147322
description: 瞭解匿名活動與人員——行銷檔案——產品檔案
title: 瞭解匿名活動與人員
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 瞭解匿名活動和人員{#understanding-anonymous-activity-and-people}

當有人第一次造訪Marketo [l `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages)（或您網站上具有[Munchkin追蹤代碼](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的頁面）時，Marketo會建立*匿名**活動*&#x200B;並使用瀏覽器Cookie來追蹤。 一旦識別後，就會變成人員，並合併與其瀏覽器Cookie相關的歷史記錄。

**當有** 人：

* 首次造訪您的Marketing登陸頁面。

* 瀏覽您網站上具有[Munchkin追蹤](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的頁面。

* 按一下行銷人員電子郵件中的[檢視為網頁](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)連結。

>[!NOTE]
>
>與Marketo電子郵件中的其他連結不同，[以網頁檢視](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)不會以電子郵件點按方式追蹤。

當某人：

* 按一下行銷人員中的[連結，以電子郵件傳送](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)。
* 填寫[Form](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)的行銷符。
* 使用Marketo的[SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846)或[Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API（開發人員），將匿名人員與已知記錄建立關聯。

資料庫中的一個名稱可能會與許多Cookie關聯，因為人們通常使用不同的裝置和瀏覽器來瀏覽您的網站。

>[!NOTE]
>
>當匿名記錄合併到新的或現有的人員記錄中時，自訂欄位值將&#x200B;**not**&#x200B;轉移。

