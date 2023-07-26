---
description: 個人帳戶同步常見問題集 — Marketo檔案 — 產品檔案
title: 個人帳戶同步常見問題集
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 個人帳戶同步常見問題集 {#person-account-sync-faq}

Marketo Engage會將您的整個資料庫與Veeva同步，以提供人員帳戶型別的記錄。 同步後，它會等待5分鐘，然後每天再次同步。

可在Veeva中設定個人帳戶，以符合貴組織的需求。

>[!NOTE]
>
>我們只將「專業」層級帳戶同步為個人帳戶。

**什麼是個人帳戶？**

個人帳戶與Veeva CRM中的帳戶物件非常類似。 不過，個人帳戶可同時存取帳戶欄位和聯絡人欄位。

**個人帳戶同步至Marketo後會發生什麼事？**

個人帳戶會以公司和個人的身分同步至Marketo。

>[!NOTE]
>
>個人帳戶的自訂欄位會複製到Marketo中的公司和個人。

**如何區分商業帳戶和個人帳戶？**

使用智慧清單中的「Is Person」帳戶篩選器，將個人帳戶與標準商業帳戶分開。

**個人帳戶應使用哪個電子郵件欄位？**

個人帳戶有兩個電子郵件欄位。 使用表單中的「電子郵件地址」欄位（而非人員電子郵件地址）來確保Marketo的重複資料刪除與其他電子郵件處理可正常運作。

## 同步方向 {#sync-direction}

同步個人帳戶的連絡人相關欄位是雙向的。 如果您在Veeva CRM或Marketo中變更連絡人，您的更新將會反映在這兩個系統中。 帳戶上的欄位只會以一個方向同步，從Veeva CRM到Marketo。

**如果在兩個系統中同時變更了人員帳戶上的聯絡人欄位，該怎麼辦？**

我們會很友善，讓Veeva CRM獲勝。 不過，這類資料衝突很少發生。

**潛在客戶或聯絡人型別的記錄是否會與Veeva CRM同步？**

Veeva CRM只真正處理個人帳戶物件，同時也擁有企業帳戶。 傳統CRM型別的Lead、Contacts和Opportunity實際上並未在傳統Veeva CRM系統中使用。 這些可在Veeva CRM中建立，但使用此聯結器並不正式支援它們。

**我可以在Marketo中將個人轉換為聯絡人嗎？**

否，因為銷售機會和連絡人不支援與Veeva CRM同步的型別。 因此，不支援轉換。

**我可以手動強制同步處理連絡人嗎？**

否，因為聯絡人不是獨立的記錄型別，所以不支援將個人同步至Veeva。

**每個標準欄位都會同步至Marketo嗎？**

否，並非所有標準欄位都有用。 所有自訂欄位都可成為同步處理的一部分。

>[!NOTE]
>
>Marketo將只會同步處理您的Marketo同步使用者有權存取的欄位。

**Marketo會遵守Veeva驗證規則嗎？**

是，如果發生衝突，我們會將結果記錄在潛在客戶的活動記錄中。

>[!MORELIKETHIS]
>
>* [預設Veeva欄位對應](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [同步呼叫和呼叫重要訊息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
