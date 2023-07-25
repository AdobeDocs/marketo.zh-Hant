---
unique-page-id: 7514918
description: 瞭解取消訂閱 — Marketo檔案 — 產品檔案
title: 瞭解取消訂閱
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# 瞭解取消訂閱 {#understanding-unsubscribe}

Marketo中實際上有數種不同型別的內建取消訂閱。 它們都由person物件上的欄位表示，就像名字一樣。

>[!NOTE]
>
>Marketo正在將產品中的黑名單和白名單等辭彙變更為封鎖名單和允許清單。 在此更新中，您可能會在UI和檔案熒幕擷取畫面中看到舊術語，並在檔案文字中看到新術語。 若有任何混淆，敬請見諒。

所有這些欄位內建在您的Marketo訂閱中。 這些全都是布林值（核取方塊）型別。 它們可以用在Forms中或 [變更資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 流程步驟。

## 退訂 {#unsubscribed}

此專案用於標準取消訂閱頁面。 如果人員核取此方塊，或按一下電子郵件中的取消訂閱連結，他們將不再收到行銷電子郵件。 但是，他們將會收到 [營運電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## 行銷活動已暫停 {#marketing-suspended}

此欄位由使用者設定，用於臨時取消訂閱人員。 只有手動變更或使用變更資料值流程步驟時，人員才能取得此狀態。

## 電子郵件已暫停 {#email-suspended}

硬跳出發生後，此狀態會在24小時內阻止個人收到郵件。 24小時後，該人員將再次變為可郵寄狀態。

>[!NOTE]
>
>即使24小時期間結束後，「已暫停的電子郵件」仍會保持檢查狀態，因此您可以指出過去曾如此標示的人員。 若要檢視該人員是否可傳送，只需在電子郵件暫停後24小時內計算即可。

## 已加入封鎖清單 {#blocklisted}

[將此用於像競爭對手這樣的人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). 您希望接收的任何人 **否** 電子郵件 — 營運、行銷等。 他們什麼也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)
