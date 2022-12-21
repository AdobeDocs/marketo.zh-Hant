---
unique-page-id: 2360181
description: 追蹤匿名活動與人員 — Marketo檔案 — 產品檔案
title: 追蹤匿名活動和人員
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 追蹤匿名活動和人員 {#tracking-anonymous-activity-and-people}

第一次有人造訪Marketo [登陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (或您網站上有 [Munchkin追蹤程式碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)),Marketo會建立 _匿名活動_ 並使用瀏覽器Cookie來追蹤。 識別訪客後，訪客就會變成人員，與瀏覽器Cookie相關聯的歷史記錄會合併。

1. 當某人：

   * 造訪您的Marketo [登陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) 第一次。
   * 瀏覽您網站上具有 [Munchkin追蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * 按一下 [作為網頁查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Marketo電子郵件中的連結。

   >[!NOTE]
   >
   >與Marketo電子郵件中的其他連結不同，以網頁形式檢視不會以電子郵件點按方式追蹤。

   當有人：

   * 點按 [Marketo電子郵件中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * 填寫Marketo [表單](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * 使用Marketo [REST API](https://developers.marketo.com/rest-api/lead-database/leads/) 或 [蒙奇金](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API（供開發人員使用），將匿名活動與已知記錄建立關聯。

   資料庫中的一個名稱可能與許多Cookie相關聯，因為人們經常使用不同的裝置和瀏覽器來造訪您的網站。

   >[!NOTE]
   >
   >當匿名記錄合併到新的或現有的人員記錄時，自訂欄位值將 **not** 轉移。

   >[!MORELIKETHIS]
   >
   >[在Web報表中顯示人員或匿名訪客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
