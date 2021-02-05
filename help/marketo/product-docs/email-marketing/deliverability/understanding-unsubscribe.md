---
unique-page-id: 7514918
description: 瞭解取消訂閱——行銷檔案——產品檔案
title: 瞭解取消訂閱
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 瞭解取消訂閱{#understanding-unsubscribe}

Marketo中實際上有幾種不同類型的內建取消訂閱。 它們都由person對象上的欄位表示，就像名字。

>[!NOTE]
>
>Marketo正在將產品中的黑名單和白名單等術語更改為區塊名單和允許名單。 在此更新期間，您可能會在我們的UI和檔案螢幕擷取畫面中看到舊有的詞語，在檔案文字中看到新的詞語。 我們為任何混淆表示歉意。

所有這些欄位都內建在您的Marketo訂閱中。 它們都是布爾型（核取方塊）類型。 它們可用於表單或[更改資料值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)流步驟。

## 取消訂閱{#unsubscribed}

這會用於標準取消訂閱頁面。 如果某人勾選此方塊，或按一下電子郵件中的取消訂閱連結，他們將不會再收到行銷電子郵件。 但是，他們會收到[操作電子郵件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

## 行銷暫停{#marketing-suspended}

此欄位由使用者設定，讓使用者暫時取消訂閱。 只有當人工變更或使用變更資料值流程步驟時，人們才能達到此狀態。

## 電子郵件已暫停{#email-suspended}

此狀態會在出現硬彈回音後，將人員封鎖24小時的郵件寄送。 24小時後，這個人將再次發郵件。

>[!NOTE]
>
>即使在24小時期間結束後，「暫停的電子郵件」仍會保持勾選狀態，因此您可以參照過去曾經標示為此類的人員。 若要查看此人是否可郵寄，只需在電子郵件暫停時24小時後計算即可。

## 列出的塊{#blocklisted}

[適用於像競爭者一樣的人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md)。您想要收到&#x200B;**no**&#x200B;電子郵件的任何人——營運、行銷等。 他們什麼也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)
