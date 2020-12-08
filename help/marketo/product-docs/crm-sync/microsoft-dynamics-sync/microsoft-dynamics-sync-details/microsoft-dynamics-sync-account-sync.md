---
unique-page-id: 3571836
description: Microsoft Dynamics Sync —— 帳戶同步——行銷人員檔案——產品檔案
title: Microsoft Dynamics Sync —— 帳戶同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Microsoft Dynamics Sync:帳戶同步 {#microsoft-dynamics-sync-account-sync}

您知道Market會將整個資料庫與Dynamics同步嗎？ 它會同步，然後等待5分鐘，然後每天再次同步。 以下是Marketo如何特別處理Dynamics帳戶的一些詳細資訊。

## 資訊會以哪種方式同步？ {#which-way-does-the-information-sync}

只有一種方式：從Dynamics到Marketo。

## 這些更新如何運作？ {#how-do-the-updates-work}

如果您更新Marketo中某個連絡人的「帳戶」欄位，則會變更Marketo中屬於該帳戶的所有連絡人的值。 它不會與Dynamics同步。 不過，下次在Dynamics中更新該帳戶時，變更將覆寫Marketo中的所有帳戶資訊。

## 我可以使用Marketo建立帳戶嗎？ {#can-i-create-an-account-using-marketo}

不。 Market無法在Dynamics中建立帳戶。

## 哪些欄位將與Marketo同步？ {#which-fields-will-sync-to-marketo}

您可以選 [取要在設定期間同步](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 的欄位。 但Marketo只會同步您的Dynamics同步使用者可存取的欄位。

## Dynamics中帳戶欄位的更改是否會為每個聯繫人生成更改資料值活動日誌？  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

大多數情況下，是的。 不過，如果帳戶有超過5,000個連絡人，而Dynamics中該帳戶的欄位變更，我們會同步變更，但不會記錄5,000個以上連絡人的活動。
