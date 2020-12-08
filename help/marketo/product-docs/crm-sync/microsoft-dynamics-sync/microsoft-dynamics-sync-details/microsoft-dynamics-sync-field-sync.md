---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs —— 產品文檔
title: Microsoft Dynamics Sync -Field Sync
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---


# Microsoft Dynamics Sync:欄位同步 {#microsoft-dynamics-sync-field-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

Marketo to Dynamics sync功能強大。 以下是詳細資訊。

## 兩個系統之間如何保持欄位詳細資訊的同步？ {#how-are-field-details-kept-in-sync-between-the-two-systems}

同步是引導實體和連絡實體的雙向同步。 如果您在Dynamics或Marketo中變更銷售線索或聯絡人，或是變更人員，您的更新將反映在這兩個系統中。

對於帳戶、用戶、機會、團隊和自定義實體，同步是單向的：Marketo的動態。 如果您在Dynamics中變更這些實體，您的更新將會反映在Marketo中。

## 如果同時對兩個系統中的同一欄位進行更改，該怎麼辦？ （資料衝突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

雖然這種情況很少見，但Marketo將贏得人（銷售機會），而Dynamics將贏得人脈。 這是因為我們認為行銷部門對人有權威性，而官方的聯絡記錄系統則位於銷售(CRM)部門。 對於單向同步實體，Dynamics將永遠勝出。

## 我可以使用Marketo在Dynamics中建立欄位嗎？ {#can-i-create-a-field-in-dynamics-using-marketo}

否，目前不支援此功能。

## 我在動力學(Dynamics)上建立了一個欄位。 我可以將它同步至Marketo嗎？ {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

是的，只要您 [的同步使用者在](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) Dynamics中擁有該欄位的存取權，您就可以同步欄位。

哪些欄位將與Marketo同步？

您可以選 [取要在設定期間同步](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 的欄位。

## 如果我需要在Marketo和Dynamics同步後新增自訂欄位，該怎麼辦？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以隨時新增欄位，並期待資料從Dynamics重新整理至Marketo。 如需詳 [細資訊，請參閱「使用與Microsoft Dynamics快速同步」以取得新的自訂欄位](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) 。

>[!NOTE]
>
>**相關文章**
>
>* [使用Quick Sync with Microsoft Dynamics，建立新的自訂欄位](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)

>



