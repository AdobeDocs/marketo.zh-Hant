---
unique-page-id: 7514918
description: 瞭解取消訂閱 — Marketo檔案 — 產品檔案
title: 了解取消訂閱
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 4%

---

# 了解取消訂閱 {#understanding-unsubscribe}

Marketo中實際上有數種不同型別的內建取消訂閱。 它們都由person物件上的欄位表示，就像「名字」一樣。

所有這些欄位都內建在您的Marketo訂閱中。 全都是布林值（核取方塊）型別。 它們可以在Forms或[變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)流程步驟中使用。

## 已取消訂閱 {#unsubscribed}

這會用於標準取消訂閱頁面。 如果人員核取此方塊，或按一下電子郵件中的取消訂閱連結，將不再收到行銷電子郵件。 但他們會收到[封營運電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

## 行銷活動暫停 {#marketing-suspended}

使用者設定此欄位，以暫時取消訂閱使用者。 只有手動變更人員或使用變更資料值流程步驟時，他們才能取得此狀態。

## 電子郵件暫停 {#email-suspended}

硬跳出發生後，此狀態會在24小時內封鎖個人傳送的郵件。 24小時後，該人員將再次變為可郵寄狀態。

>[!NOTE]
>
>即使24小時期間結束後，系統仍會檢查「已暫停的電子郵件」，因此您可以指出過去曾如此標示的人。 若要檢視該人員是否可郵寄，只需在電子郵件暫停時間24小時後計算即可。

## 已加入封鎖清單 {#blocklisted}

[將此用於競爭者之類的人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md)。 任何您想要接收&#x200B;**no**&#x200B;電子郵件的人 — 營運、行銷等 他們什麼也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)
