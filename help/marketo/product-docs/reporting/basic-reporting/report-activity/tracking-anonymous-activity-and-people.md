---
unique-page-id: 2360181
description: 追蹤匿名活動和人員 — Marketo檔案 — 產品檔案
title: 追蹤匿名活動和人員
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 追蹤匿名活動和人員 {#tracking-anonymous-activity-and-people}

第一次有人造訪Marketo [登陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) （或您的網站上具有[Munchkin追蹤代碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的頁面）時，Marketo會建立&#x200B;_匿名活動_&#x200B;並使用瀏覽器Cookie進行追蹤。 在識別訪客後，訪客會變成人員，且與瀏覽器Cookie相關的歷史記錄會合併到中。

1. 當有人員符合以下條件時，則會建立匿名活動：

   * 第一次造訪您的Marketo [登陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)。
   * 瀏覽網站上具有[Munchkin追蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的頁面。
   * 按一下Marketo電子郵件中的[以網頁形式檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)連結。

   >[!NOTE]
   >
   >與Marketo電子郵件中的其他連結不同，以網頁檢視不會以電子郵件點按追蹤。

   在下列情況下，匿名活動會合併至新的或現有人員：

   * 按一下Marketo電子郵件[&#128279;](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)中的連結。
   * 填寫Marketo [表單](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)。
   * 使用Marketo的[REST API](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/lead-database/leads)或[Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking) API （適用於開發人員），將匿名活動與已知記錄建立關聯。

   資料庫中的一個名稱可能與許多Cookie繫結，因為人們經常使用不同的裝置和瀏覽器來造訪您的網站。

   >[!NOTE]
   >
   >將匿名記錄合併至新的或現有的人員記錄時，自訂欄位值將&#x200B;**不會**&#x200B;移轉。

   >[!MORELIKETHIS]
   >
   >[顯示網路報表中的人員或匿名訪客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
