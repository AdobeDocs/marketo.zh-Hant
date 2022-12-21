---
unique-page-id: 2953461
description: SFDC同步 — 欄位同步 — Marketo文檔 — 產品文檔
title: SFDC同步 — 欄位同步
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# SFDC同步：欄位同步 {#sfdc-sync-field-sync}

Marketo會同步Salesforce的欄位資訊。 詳情如下。

## 要同步哪些欄位？ {#which-fields-are-synced}

我們同步了SFDC中的大多數標準欄位以及同步用戶有權查看的任何自定義欄位。

## 如何判斷Marketo中的記錄是銷售機會還是Salesforce中的聯絡人？ {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Marketo中有一個名為SFDC Type的欄位。 它有三個可能的值：線索，聯繫，或者是空的。 如果空白，表示此Marketo銷售機會在SFDC中不存在。

## 如何確定SFDC中是否刪除了銷售機會或聯繫人？ {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Marketo中有一個名為SFDC isDeleted的欄位。 如果值為true，則銷售機會在SFDC中被刪除。

## 如何確保在SFDC中新增的新欄位也新增至Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>如果要在兩個系統中建立一個欄位，請先在SFDC中建立該欄位，該欄位將自動同步到Marketo。

如果您在SFDC中新增欄位，且同步使用者有權查看，則會自動將其新增至Marketo。

## 如果在SFDC中更改欄位標籤，該怎麼辦？ {#what-if-i-change-a-field-label-in-sfdc}

在SFDC中變更欄位標籤不會影響Marketo中的欄位標籤。

## 如果在SFDC中更改欄位類型，該怎麼辦？ {#what-if-i-change-a-field-type-in-sfdc}

變更欄位類型時，如果欄位中的資料不相符，Marketo會刪除這些資料（但會先顯示警告）。 若要保留資料，請務必在變更欄位類型後將其匯出並重新匯入。

## 如果我在SFDC中變更API名稱，該怎麼辦？ {#what-if-i-change-an-api-name-in-sfdc}

如果您變更SFDC中欄位的API名稱，則會在Marketo中建立新欄位。

## 如果在SFDC中添加新的選擇清單值，會發生什麼情況？ {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

如果在SFDC中將新的選擇清單值添加到欄位，Marketo將向您發送通知。

## 自訂SFDC查閱欄位有什麼變化？ {#what-about-custom-sfdc-lookup-fields}

SFDC中的查找欄位會同步ID，但不同步引用的名稱。

## SFDC公式欄位呢？ {#what-about-sfdc-formula-fields}

不過，系統會同步公式欄位，但是在更新 [系統模式戳](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## 從先前與Marketo同步的Salesforce刪除欄位時會發生什麼事？ {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

如果您刪除SFDC中的欄位，它不會自動刪除Marketo中的欄位，只會停止同步。
