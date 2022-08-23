---
unique-page-id: 1147322
description: 瞭解匿名活動和人員 — Marketo文檔 — 產品文檔
title: 理解匿名活動與人
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
source-git-commit: cc66f4ff2e3e0e6ddfabab91215e3ad31f3b9226
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 理解匿名活動與人 {#understanding-anonymous-activity-and-people}

第一次有人訪問Marketo登錄頁(或您網站上 [Munchkin跟蹤代碼](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md),Marketo建立 _匿名活動_ 用瀏覽器cookie來跟蹤。 一旦標識它，它就成為人員，並且與其瀏覽器cookie關聯的歷史記錄將合併到中。

>[!IMPORTANT]
>
>啟用Beta功能 **已知的Munchkin V2匿名重播活動** 確保在匿名線索成功合併到已知記錄後，將始終重播由匿名線索促銷觸發的市場活動。 因此，任何重播市場活動中由「更改資料值」步驟更改的自定義欄位將保留在已知記錄中。

**匿名** 當某人：

* 第一次訪問您的Marketo登錄頁。
* 訪問您站點上具有 [蒙奇金跟蹤](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)。
* 按一下 [作為網頁查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 連結到Marketo的電子郵件。

>[!NOTE]
>
>與Marketo郵件中的其他連結不同， [作為網頁查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 未作為電子郵件按一下跟蹤。

當某人：

* 按一下 [在Marketo的電子郵件中連結](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)。
* 填滿Marketo [窗體](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)。
* 使用Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) 或 [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 用於將匿名人員與已知記錄關聯的API。

資料庫中的一個名稱可能與許多cookie相關，因為人們通常使用不同的設備和瀏覽器訪問您的站點。

>[!NOTE]
>
>當匿名記錄合併到新的或現有的人員記錄中時，自定義欄位值將 **不** 轉移。
