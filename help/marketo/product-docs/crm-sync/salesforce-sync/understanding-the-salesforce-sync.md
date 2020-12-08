---
unique-page-id: 4719283
description: 瞭解Salesforce同步——行銷檔案——產品檔案
title: 瞭解Salesforce同步
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 瞭解Salesforce同步 {#understanding-the-salesforce-sync}

Marketo和Salesforce像豌豆和胡蘿蔔一樣合作。 我們讓您的銷售和行銷資料保持同步。

## 同步的運作方式 {#how-sync-works}

Market每天都會與Salesforce同步。 每次同步都需要一段時間，然後暫停5分鐘，然後再次開始。

>[!NOTE]
>
>您的訂閱中第一次同步可能需要數小時甚至數天，因為Marketo正從Salesforce複製整個資料庫。 之後，每次同步通常需要數秒或數分鐘，而且只同步已變更的資料。

![](assets/sync-illustration.png)

Salesforce和Marketo之間的同步僅適用於潛在客戶、連絡人和Salesforce促銷活動。 在這些情況下，每當您在Salesforce或Marketo中進行變更時，您的更新都會反映在這兩種系統中。 所有其他同步都只從Salesforce到Marketo。 按一下下列連結，以取得每個連結的詳細資訊。

## Marketo和Salesforce之間有何同步？ {#what-is-synced-between-marketo-and-salesforce}

* [銷售線索](sfdc-sync-details/sfdc-sync-lead-sync.md)
* [聯絡人](sfdc-sync-details/sfdc-sync-contact-sync.md)
* [帳戶](sfdc-sync-details/sfdc-sync-account-sync.md)
* [使用者](sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [機會](sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce促銷活動](sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [自訂物件](sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [活動](sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>您 [在Marketo中為Salesforce輸入的認證](setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) ，用於同步資料。 只有這些認證有權存取的資料才會包含在內。

Salesforce同步有許多細微差別和功能。 查看 [SFDC同步詳細資訊部分中的詳細資訊](http://docs.marketo.com/display/docs/sfdc+sync+details)。

>[!NOTE]
>
>**相關文章**
>
>* [Salesforce同步設定](http://docs.marketo.com/display/docs/setup)
>* [SFDC同步詳細資訊](http://docs.marketo.com/display/docs/sfdc+sync+details)

>



Marketo與Salesforce的同步性是全球同類產品中最強大的。 這感覺就像魔術一樣——一項改變已經完成，而另一項系統也很快就是最新版本。