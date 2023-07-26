---
unique-page-id: 2953461
description: SFDC同步 — 欄位同步 — Marketo檔案 — 產品檔案
title: SFDC同步 — 欄位同步
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# SFDC同步：欄位同步 {#sfdc-sync-field-sync}

Marketo會從Salesforce同步欄位資訊。 詳情如下。

## 哪些欄位已同步？ {#which-fields-are-synced}

我們會同步SFDC中大部分的標準欄位，以及同步使用者有權檢視的任何自訂欄位。

## 如何判斷Marketo中的記錄是Salesforce中的潛在客戶或聯絡人？ {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Marketo中有一個名為「SFDC型別」的欄位。 它有三個可能的值：銷售機會、聯絡人，或空白。 如果空白，表示此Marketo銷售機會不存在於SFDC中。

## 如何判斷在SFDC中是否刪除潛在客戶或連絡人？ {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Marketo中有一個名為SFDC isDeleted的欄位。 如果值為true，則在SFDC中刪除潛在客戶。

## 如何確定我在SFDC中新增的新欄位也會新增至Marketo？ {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>如果您想要在兩個系統中都使用一個欄位，請先在SFDC中建立該欄位，它會自動同步至Marketo。

如果您在SFDC中新增欄位，且同步使用者有權檢視該欄位，該欄位會自動新增至Marketo。

## 如果我變更SFDC中的欄位標籤，該怎麼辦？ {#what-if-i-change-a-field-label-in-sfdc}

變更SFDC中的欄位標籤不會影響Marketo中的欄位標籤。

## 如果我變更SFDC中的欄位型別，該怎麼辦？ {#what-if-i-change-a-field-type-in-sfdc}

當您變更欄位型別時，如果欄位中的資料不符，Marketo會將其刪除（但會先顯示警告）。 若要保留資料，請務必匯出資料，並在變更欄位型別後重新匯入資料。

## 如果我在SFDC中變更API名稱，該怎麼辦？ {#what-if-i-change-an-api-name-in-sfdc}

如果您變更SFDC中欄位的API名稱，則會在Marketo中建立新欄位。

## 如果我在SFDC中新增挑選清單值，會發生什麼事？ {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

如果在SFDC中將新的挑選清單值新增至欄位，Marketo會傳送通知給您。

## 自訂SFDC查閱欄位呢？ {#what-about-custom-sfdc-lookup-fields}

SFDC中的查閱欄位會同步ID，但不會同步參照的名稱。

## SFDC公式欄位呢？ {#what-about-sfdc-formula-fields}

公式欄位會同步，但公式中參照的更新要等到更新後才會同步。 [系統模組戳記](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## 當我從Salesforce中刪除先前與Marketo同步的欄位時，會發生什麼情況？ {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

如果您刪除SFDC中的欄位，並不會自動刪除Marketo中的欄位，而只會停止同步。
