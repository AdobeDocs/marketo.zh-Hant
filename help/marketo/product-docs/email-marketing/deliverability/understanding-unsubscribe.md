---
unique-page-id: 7514918
description: 了解取消訂閱 — Marketo檔案 — 產品檔案
title: 了解取消訂閱
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# 了解取消訂閱 {#understanding-unsubscribe}

Marketo中實際上有數種不同類型的內建取消訂閱。 它們都由人員物件上的欄位表示，就像「名字」一樣。

>[!NOTE]
>
>Marketo正在將產品中的黑名單和白名單等詞語變更為封鎖名單和允許清單。 在此更新期間，您可能會在UI和檔案螢幕擷取畫面中看到舊辭彙，並在檔案文字中看到新辭彙。 我們為任何混淆道歉。

所有這些欄位都內建在您的Marketo訂閱中。 這些都是布林值（核取方塊）類型。 它們可用於Forms或 [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 流程步驟。

## 退訂 {#unsubscribed}

這會用於標準的取消訂閱頁面。 如果使用者勾選此方塊，或按一下電子郵件中的取消訂閱連結，將不再收到行銷電子郵件。 但是，他們將獲得 [操作電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## 行銷活動已暫停 {#marketing-suspended}

此欄位由使用者設定，用於讓使用者暫時取消訂閱。 只有在手動更改或使用更改資料值流步驟時，才能達到此狀態。

## 電子郵件已暫停 {#email-suspended}

此狀態會在發生硬退信後24小時封鎖某人的郵件。 24小時後，該人將再次發郵件。

>[!NOTE]
>
>即使24小時期間結束後，「暫停的電子郵件」仍會維持勾選狀態，因此您可以指出過去已標示為此類的使用者。 若要查看該人是否有郵件，只需在電子郵件暫停時計算24小時即可。

## 已列入封鎖名單 {#blocklisted}

[將此功能用於競爭者等使用者](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). 任何你想接受的人 **no** 電子郵件 — 操作、行銷等 他們什麼也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)
