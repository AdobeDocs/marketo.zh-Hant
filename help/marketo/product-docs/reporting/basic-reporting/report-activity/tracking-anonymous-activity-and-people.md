---
unique-page-id: 2360181
description: 追蹤匿名活動和人員 — Marketo檔案 — 產品檔案
title: 追蹤匿名活動和人員
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 追蹤匿名活動和人員 {#tracking-anonymous-activity-and-people}

第一次有人造訪Marketo時 [登陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (或您網站上具有下列專案的頁面： [Munchkin追蹤程式碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md))，Marketo會建立 _匿名活動_ 並使用瀏覽器Cookie加以追蹤。 在識別訪客後，訪客會變成人員，且與瀏覽器Cookie相關的歷史記錄會合併到中。

1. 當有人員符合以下條件時，則會建立匿名活動：

   * 造訪您的Marketo [登陸頁面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) 第一次。
   * 造訪您網站上具有 [Munchkin追蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * 按一下 [以網頁檢視](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Marketo電子郵件中的連結。

   >[!NOTE]
   >
   >與Marketo電子郵件中的其他連結不同，以網頁檢視不會以電子郵件點按追蹤。

   在下列情況下，匿名活動會合併至新的或現有人員：

   * 按一下 [Marketo電子郵件中的連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * 填寫Marketo [表單](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * 使用Marketo的 [REST API](https://developers.marketo.com/rest-api/lead-database/leads/) 或 [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API （適用於開發人員），將匿名活動與已知記錄建立關聯。

   資料庫中的一個名稱可能與許多Cookie繫結，因為人們經常使用不同的裝置和瀏覽器來造訪您的網站。

   >[!NOTE]
   >
   >將匿名記錄合併至新的或現有的個人記錄時，自訂欄位值將 **非** 移轉過去。

   >[!MORELIKETHIS]
   >
   >[在網頁報表中顯示人員或匿名訪客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
