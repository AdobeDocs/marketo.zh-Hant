---
description: 回復日誌 — Marketo文檔 — 產品文檔
title: 回復日誌記錄
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# 回復日誌記錄 {#reply-logging}

Sales Insight Actions使您能夠自動記錄潛在客戶對Salesforce的答復。 允許您執行此操作的結構基於我們的電子郵件回復跟蹤。 如果我們可以跟蹤潛在客戶的回復，我們可以將該回復記錄到Salesforce。

## 要求 {#requirements}

* 必須通過API日誌記錄電子郵件
* 必須能夠 [跟蹤回復](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* 必須與Salesforce連接
* 必須有Salesforce [API調用](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) 可用

## 啟用回復日誌記錄 {#enable-reply-logging}

1. 要啟用回復日誌記錄，您可以轉到Salesforce設定頁。 一旦API日誌記錄被勾選，您將看到選項以勾選 _日誌答復_。

   >[!NOTE]
   >
   >回復日誌記錄遵循與記錄發送的電子郵件相同的規則。 這包括電子郵件的記錄方式；到Lead和Contacts;有重複記錄的；找不到匹配記錄。

## 在Salesforce中將類型設定為回復 {#setting-type-to-reply-in-salesforce}

從Salesforce報告中獲取有意義的資料非常重要。 如果能夠將「類型」欄位填充為「答復」，則可以通過報告獲取該資料。 與您的 `Salesforce admin` 來設定。

1. 轉到 **設定** > **自定義** > **活動** > **任務欄位**。
1. 按一下 **類型**。
1. 在任務類型選擇清單值下，按一下 **新建**。
1. 在空框中鍵入「Reply」。 確保將「R」大寫，然後按一下 **保存**。

   >[!NOTE]
   >
   >您無需在「類型」(Type)選擇清單下選擇「預設」(Default)。 Sales Insight Actions將查看此活動類型在您的Salesforce實例中可用，並相應地填充傳入活動的任務欄位。
