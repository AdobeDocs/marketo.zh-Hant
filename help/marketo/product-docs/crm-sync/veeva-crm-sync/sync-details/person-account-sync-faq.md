---
description: 人員帳戶同步常見問題集 — Marketo檔案 — 產品檔案
title: 人員帳戶同步常見問題集
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# 人員帳戶同步常見問題集 {#person-account-sync-faq}

Marketo Engage會針對「人員帳戶」類型的記錄，使用Veva同步整個資料庫。 同步後會等待5分鐘，然後每天再次同步。

您可以在Veeva中設定人員帳戶，以符合您組織的需求。

>[!NOTE]
>
>我們只將「專業」層帳戶同步為「人員帳戶」。

**什麼是人員帳戶？**

人員帳戶與Veeva CRM中的帳戶物件非常類似。 但是，人員帳戶可以同時訪問帳戶欄位和聯繫人欄位。

**將人員帳戶同步至Marketo時會發生什麼事？**

人員帳戶會以公司和人員身分同步至Marketo。

>[!NOTE]
>
>人員帳戶的自訂欄位會複製到Marketo中的公司和人員。

**如何區分業務帳戶和人員帳戶？**

使用智慧清單中的「是人」帳戶篩選器，將人員帳戶與標準業務帳戶分開。

**我應將哪個電子郵件欄位用於人員帳戶？**

人員帳戶有兩個電子郵件欄位。 使用表單中的「電子郵件地址」欄位（而非「人員電子郵件地址」），確保Marketo的重複資料消除和其他電子郵件處理正常運作。

## 同步方向 {#sync-direction}

「人員帳戶」的聯繫人相關欄位的同步是雙向的。 如果您在Veva CRM或Marketo中變更連絡人，您的更新將會反映在這兩個系統中。 帳戶上的欄位只會從Veva CRM同步至Marketo。

**如果同時在兩個系統中對「人員帳戶」的「聯繫人」欄位進行更改，該怎麼辦？**

我們會很友好，讓維娃CRM贏。 然而，這種資料衝突很少發生。

**與Veva CRM同步的記錄的銷售機會或聯絡人類型？**

Veva CRM只真正處理「人員帳戶」對象，也有「業務帳戶」。 傳統的CRM類型的Lead 、 Contacts和Opportunity在傳統的Veeva CRM系統中沒有真正使用。 這些變數可在Veeva CRM中建立，但未正式使用此連接器支援。

**我可以在Marketo將人員轉換為聯絡人嗎？**

否，因為與Veeva CRM同步時不支援銷售機會和聯絡人類型。 因此，不支援轉換。

**我可以手動強制同步連絡人嗎？**

否，由於「聯絡人」不是獨立的記錄類型，因此不支援將人員同步至Veeva。

**每個標準欄位都會同步至Marketo嗎？**

不，並非所有標準欄位都有用。 所有自訂欄位都可以是同步的一部分。

>[!NOTE]
>
>Marketo只會同步您的Marketo同步使用者有權存取的欄位。

**Marketo會遵守Veeva驗證規則嗎？**

是，如果發生衝突，我們會將結果記錄在銷售機會的活動記錄中。

>[!MORELIKETHIS]
>
>* [預設Veeva欄位映射](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target=&quot;_blank&quot;}
>* [正在同步呼叫和呼叫密鑰消息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}

