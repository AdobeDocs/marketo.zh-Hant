---
description: 個人帳戶同步常見問題集 — Marketo檔案 — 產品檔案
title: 個人帳戶同步常見問題集
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 個人帳戶同步常見問題集 {#person-account-sync-faq}

Marketo Engage會針對個人帳戶型別的記錄，將整個資料庫與[!DNL Veeva]同步。 同步後，它會等待5分鐘，然後每天再次同步。

個人帳戶可在[!DNL Veeva]中設定以符合您組織的需求。

>[!NOTE]
>
>我們只將「專業」層級帳戶同步為個人帳戶。

**什麼是個人帳戶？**

個人帳戶與[!DNL Veeva] CRM中的帳戶物件非常類似。 不過，個人帳戶可同時存取帳戶欄位和聯絡人欄位。

**當個人帳戶同步至Marketo時會發生什麼事？**

個人帳戶會以公司和個人的身分同步至Marketo。

>[!NOTE]
>
>個人帳戶的自訂欄位會複製到Marketo中的公司和個人。

**如何區分商業帳戶和個人帳戶？**

使用智慧清單中的「Is Person」帳戶篩選器，將個人帳戶與標準商業帳戶分開。

**我該使用哪個電子郵件欄位作為個人帳戶？**

個人帳戶有兩個電子郵件欄位。 使用表單中的「電子郵件地址」欄位（而非人員電子郵件地址）來確保Marketo的重複資料刪除與其他電子郵件處理可正常運作。

## 同步方向 {#sync-direction}

同步個人帳戶的連絡人相關欄位是雙向的。 如果您在[!DNL Veeva] CRM或Marketo中變更連絡人，您的更新將會反映在這兩個系統中。 帳戶上的欄位只會同步到一個方向，從[!DNL Veeva] CRM到Marketo。

**如果在兩個系統中同時變更人員帳戶上的連絡人欄位，該怎麼辦？**

我們會很友善，讓[!DNL Veeva] CRM獲勝。 不過，這類資料衝突很少發生。

**記錄的潛在客戶或連絡人型別是否已與[!DNL Veeva] CRM同步？**

[!DNL Veeva] CRM只真正處理個人帳戶物件，並且也有企業帳戶。 傳統CRM型別的Lead、Contacts和Opportunity實際上並未在傳統[!DNL Veeva] CRM系統中使用。 這些可在[!DNL Veeva] CRM中建立，但使用此聯結器並不正式支援它們。

**我可以在Marketo中將某人轉換為聯絡人嗎？**

否，因為潛在客戶與連絡人不支援與[!DNL Veeva] CRM同步處理的型別。 因此，不支援轉換。

**我可以手動強制同步處理連絡人嗎？**

否，因為連絡人不是獨立的記錄型別，所以不支援將人員同步至[!DNL Veeva]。

**每個標準欄位是否都會同步至Marketo？**

否，並非所有標準欄位都有用。 所有自訂欄位都可成為同步處理的一部分。

>[!NOTE]
>
>Marketo將只會同步處理您的Marketo同步使用者有權存取的欄位。

**Marketo是否會遵守[!DNL Veeva]驗證規則？**

是，如果發生衝突，我們會將結果記錄在潛在客戶的活動記錄中。

>[!MORELIKETHIS]
>
>* [預設 [!DNL Veeva] 欄位對應](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [正在同步通話和通話主要訊息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
