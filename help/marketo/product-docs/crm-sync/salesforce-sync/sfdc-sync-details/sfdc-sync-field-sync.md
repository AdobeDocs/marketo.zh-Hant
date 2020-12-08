---
unique-page-id: 2953461
description: SFDC同步——現場同步——行銷文檔——產品文檔
title: SFDC同步——欄位同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# SFDC同步：欄位同步 {#sfdc-sync-field-sync}

Marketo會同步來自Salesforce的欄位資訊。 以下是詳細資訊。

## 哪些欄位已同步？ {#which-fields-are-synced}

我們同步SFDC中的大多數標準欄位以及同步用戶有權查看的任何自定義欄位。

## 您如何判斷Marketo中的記錄是Salesforce中的潛在客戶或連絡人？ {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

我們在Marketo中有一個欄位，叫做SFDC Type。 它有三個可能的值：線索，聯繫，或者是空的。 如果是空的，表示此Marketo銷售線索在SFDC中不存在。

## 如何確定SFDC中是否刪除了銷售線索或聯繫人？ {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

我們在Marketo中有一個名為SFDC isDeleted的欄位。 如果值為true，則SFDC中的銷售線索被刪除。

## 如何確保在SFDC中添加的新欄位也添加到Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>如果您想要在兩個系統中都有一個欄位，請先在SFDC中建立欄位，並自動同步至Marketo。

如果您在SFDC中新增欄位，而同步使用者有權查看，則會自動新增至Marketo。

## 如果我更改了SFDC中的欄位標籤，該怎麼辦？ {#what-if-i-change-a-field-label-in-sfdc}

變更SFDC中的欄位標籤不會影響Marketo中的欄位標籤。

## 如果我更改了SFDC中的欄位類型，該怎麼辦？ {#what-if-i-change-a-field-type-in-sfdc}

當您變更欄位類型時，Marketo會在欄位中刪除不符合的資料（但會先顯示警告）。 若要保留資料，請務必在變更欄位類型後匯出並重新匯入。

## 如果我在SFDC中更改了API名稱，該怎麼辦？ {#what-if-i-change-an-api-name-in-sfdc}

如果您變更SFDC中欄位的API名稱，Marketo中會建立新欄位。

## 如果我在SFDC中添加新的選擇清單值，會發生什麼情況？ {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

如果SFDC中新增選取清單值至欄位，Marketo會傳送通知給您。

## 自訂SFDC查閱欄位如何？ {#what-about-custom-sfdc-lookup-fields}

SFDC中的查閱欄位會同步ID，但不會同步參考的名稱。

## SFDC公式欄位如何？ {#what-about-sfdc-formula-fields}

但公式欄位會同步，直到系統模組戳記更新為止，公式中參考的更新才會 [同步](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US)。

## 當我從Salesforce刪除先前與Marketo同步的欄位時，會發生什麼情況？ {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

如果您刪除SFDC中的欄位，並不會自動刪除Marketo中的欄位，只會停止同步。
