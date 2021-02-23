---
unique-page-id: 2360181
description: 追蹤匿名活動與人員——行銷檔案——產品檔案
title: 追蹤匿名活動與人員
translation-type: tm+mt
source-git-commit: 03ee7b69f691efce12825aa708c81dffa23cecd9
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---


# 追蹤匿名活動與人員{#tracking-anonymous-activity-and-people}

當有人第一次造訪Marketo [著陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)（或您網站上具有[Munchkin追蹤代碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的頁面）時，Marketo會建立&#x200B;_匿名活動_，並使用瀏覽器Cookie來追蹤。 一旦識別訪客後，該訪客就會變成人員，而與瀏覽器Cookie相關的歷史記錄會合併在中。

1. 當有人：

   * 首次造訪您的行銷人員至[著陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)。
   * 瀏覽您網站上具有[Munchkin追蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的頁面。
   * 按一下行銷人員電子郵件中的[檢視為網頁](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)連結。

   >[!NOTE]
   >
   >與Marketo電子郵件中的其他連結不同，「以網頁形式檢視」不會以電子郵件點按方式追蹤。

   當某人：

   * 按一下行銷人員中的[連結，以電子郵件傳送](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)。
   * 填寫[form](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)的行銷工具。
   * 使用Marketo的[REST API](https://developers.marketo.com/rest-api/lead-database/leads/)或[Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API（開發人員），將匿名活動與已知記錄建立關聯。

   資料庫中的一個名稱可能會與許多Cookie關聯，因為人們通常使用不同的裝置和瀏覽器來瀏覽您的網站。

   >[!NOTE]
   >
   >當匿名記錄合併到新的或現有的人員記錄中時，自訂欄位值將&#x200B;**not**&#x200B;轉移。

   >[!MORELIKETHIS]
   >
   >[在Web報表中顯示人物或匿名訪客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
