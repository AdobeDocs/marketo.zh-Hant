---
description: 人員客戶同步常見問題 — Marketo文檔 — 產品文檔
title: 人員帳戶同步常見問題
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 人員帳戶同步常見問題 {#person-account-sync-faq}

Marketo Engage將整個資料庫與Veeva同步，以便記錄的「人員帳戶」類型。 同步後，它等待5分鐘，然後每天再次同步。

可以在Veeva中設定人員帳戶，以滿足您組織的需要。

>[!NOTE]
>
>預設的Veeva帳戶是Professionals。

**什麼是個人帳戶？**

人員帳戶與Veeva CRM中的帳戶對象非常相似。 但是，個人帳戶可以訪問帳戶欄位和聯繫人欄位。

**當人員帳戶同步到Marketo時會發生什麼？**

人員帳戶與Marketo同步為公司和人員。

>[!NOTE]
>
>個人帳戶的自定義欄位將複製到Marketo的公司和個人。

**如何區分業務客戶和個人客戶？**

使用智慧清單中的「是人」帳戶篩選器將人員帳戶與標準業務帳戶分開。

**我應將哪個電子郵件欄位用於個人帳戶？**

個人帳戶有兩個電子郵件欄位。 使用表單中的「電子郵件地址」欄位（而非「個人電子郵件地址」），確保Marketo的重複資料消除和其他電子郵件處理工作正常。

## 同步方向 {#sync-direction}

人員帳戶的聯繫人相關欄位的同步是雙向的。 如果您在Veeva CRM或Marketo中對聯繫人進行了更改，您的更新將反映在兩個系統中。 帳戶上的欄位只沿一個方向同步，從Veeva CRM到Marketo。

**如果在兩個系統中同時對「人員帳戶」上的「聯繫人」欄位進行更改，會如何？**

我們會很友好，讓維娃CRM贏。 然而，這種資料衝突很少發生。

**是否與Veeva CRM同步的記錄的潛在客戶或聯繫人類型？**

Veeva CRM只真正處理Person Account對象，還有Business Accounts。 傳統的CRM類型的Lead 、 Contacts和Opportunity在傳統的Veeva CRM系統中並沒有真正使用。 這些內容可能在Veeva CRM中建立，同步可能會將它們帶入Marketo，但是使用此連接器不受正式支援。

**我能把一個人變成Marketo的聯繫人嗎？**

否，因為Lead和Contact不支援與Veeva CRM同步的類型。 因此，不支援轉換。

**是否可以手動強制同步聯繫人？**

否，因為Contact不是獨立的記錄類型，因此不支援將人員同步到Veeva。

**每個標準欄位都與Marketo同步嗎？**

不，並非所有標準欄位都有用。 所有自定義欄位都可以是同步的一部分。

>[!NOTE]
>
>Marketo將僅同步您的Marketo同步用戶有權訪問的欄位。

**Marketo會遵守維娃的驗證規則嗎？**

是的，如果存在衝突，我們將將結果記錄在潛在客戶的活動日誌中。

>[!MORELIKETHIS]
>
>* [預設Veeva欄位映射](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target=&quot;_blank&quot;
>* [同步呼叫和呼叫密鑰消息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;

