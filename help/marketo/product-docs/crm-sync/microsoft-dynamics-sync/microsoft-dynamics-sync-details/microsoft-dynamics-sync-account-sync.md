---
unique-page-id: 3571836
description: Microsoft Dynamics Sync —— 帳戶同步-Marketo文檔——產品文檔
title: Microsoft Dynamics Sync —— 帳戶同步
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics Sync:帳戶同步{#microsoft-dynamics-sync-account-sync}

您知道Marketo將您的整個資料庫與Dynamics同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是有關Marketo如何具體處理動態帳戶的一些詳細資訊。

## 資訊會以哪種方式同步？{#which-way-does-the-information-sync}

只有一種方式：從動力學到Marketo。

## 這些更新如何運作？{#how-do-the-updates-work}

如果您更新了Marketo地區某個聯繫人的「帳戶」欄位，則它將更改屬於Marketo地區該帳戶的所有聯繫人的值。 它不會與Dynamics同步。 不過，下次在Dynamics中更新該帳戶時，變更將覆寫Marketo的所有帳戶資訊。

## 我可以使用Marketo建立帳戶嗎？{#can-i-create-an-account-using-marketo}

不。 Marketo無法在Dynamics中建立帳戶。

## 哪些欄位會與Marketo同步？{#which-fields-will-sync-to-marketo}

您可以在設定期間選取要同步的欄位。 [](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)但Marketo將只同步您的Dynamics同步使用者可存取的欄位。

## Dynamics中帳戶欄位的更改是否會為每個聯繫人生成更改資料值活動日誌？ {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

大多數情況下，是的。 不過，如果帳戶有超過5,000個連絡人，而Dynamics中該帳戶的欄位變更，我們會同步變更，但不會記錄5,000個以上連絡人的活動。
