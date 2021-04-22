---
unique-page-id: 45416698
description: 發行說明- 2007年7月-Marketo文檔——產品文檔
title: 發行說明- 2002年7月
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# 發行說明：7月20日{#release-notes-july}

7月20日發行包含下列功能。 查看您的Marketo版功能是否可用。

>[!AVAILABILITY]
>
>請注意，視您目前的套件而定，含星號(![(star)](assets/star-yellow.svg))的項目可能需要購買附加值。 請連絡您的Marketo Engage代表以瞭解更多資訊。

**_季_** 度發行以下功能將於2020年7 **月31日發行**。

## 管理{#administration}

* **[欄位管理中的「使用者」匯出](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**:管理員現在可將選取欄位的所有「使用者」資產連結匯出為CSV檔案。此增強功能可協助管理員和非管理員清除未使用的欄位。 此外，資產現在可以在新的瀏覽器標籤或視窗中開啟。

## 帳戶型行銷{#account-based-marketing}

![（星號）](assets/star-yellow.svg)

* **更新帳戶分析的UI**:在「帳戶分析」中，透過單一畫面中簡化的步驟，簡化目標帳戶清單的建立程式。

<br> 

**_整季發行_**

以下功能是非季度週期，將於未來數月內發佈。

* **Forms社**:我們推出更強大的表單欄位語法驗證功能，並透過新的著陸頁面安全網域功能來封鎖常見的機器人模式。封鎖機器人模式可以減少垃圾訊息提交，並改善資料庫品質。

>[!NOTE]
>
>增強表單欄位語法驗證的完整推出已推遲至2021年1月發行後。

* **增加資產API URI大小限制**:在刪除&quot;_method&quot;參數之前，統一資源標識符(URI)大小限制從8KB增加到65KB。執行長查詢字串時，此大小限制的增加可讓資料更容易傳遞。 移除&quot;_method&quot;參數是即將進行的安全性升級的一部份。

## 銷售分析{#sales-insight}

![（星號）](assets/star-yellow.svg)

* **[針對非原生Salesforce CRM整合](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) （測試版）的客戶啟用銷售洞察**:具有非原生Salesforce CRM整合的Marketo Engage客戶現在可以使用Sales Insight來協助其銷售團隊瞭解、排定優先順序，並與最具吸引力的客戶和機會互動，以實現智慧銷售和更快的交易。

## 銷售連接{#sales-connect}

![（星號）](assets/star-yellow.svg)

* **[增強銷售電話的雙方同意：管](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** 理員現在更能控制電話錄制組態。[您可以](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) 確信您符合雙方同意法，啟用通話記錄。自動記錄通話的通知，並啟用通話前要播放的音訊片段。

<br> 

## 公告與淘汰{#announcements-deprecations}

* **資產API &quot;_method&quot;參數移除**:在2020年9月之後，資產API端點將不再接受&quot;_method&quot;來傳遞POST內文中的查詢參數，以略過URI長度限制。為配合需要此參數的要求，資產API的URI限制將從8KB增加為65KB。
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:在本版Munchkin JavaScript用戶端159版中，我們將開始淘汰Munchkin Associate Lead方法。如果呼叫，您會收到警告，指出該方法將在未來版本中移除。 移除後，方法將不再正常運作，且嘗試使用方法將失敗。 Marketo Engage客戶若最近使用此方法，將會個別收到使用通知。
* **支援Internet Explorer**:如先前所宣佈，Marketo Engage對Internet Explorer 11的支援將於2020 **年7月31日截止**。我們將繼續支援Google Chrome、Mozilla Firefox、Apple Safari和Microsoft Edge。
* **Sky預設體驗**:此版本將移除管理員或使用者將Marketo Sky設為預設體驗的選項，以備主要使用者體驗的更新。預計在今年晚些時候推出的主要體驗更新的更多詳細資訊將於7月推出。 已將Marketo Sky設為預設體驗或已授與Marketo Sky存取權的使用者，可繼續從「我的Marketo」首頁的方塊存取Marketo Sky。
* **EdgeHTML（非Chromium）Microsoft Edge支援**:Marketo Engage將於2020年底不再支援Microsoft Edge的EdgeHTML版本。從2021年1月1日開始，我們將只支援最新版Chromium Edge。
