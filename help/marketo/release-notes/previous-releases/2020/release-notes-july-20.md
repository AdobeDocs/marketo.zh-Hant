---
unique-page-id: 45416698
description: 發行說明 — 2020年7月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年7月
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# 發行說明：』20年7月 {#release-notes-july}

』20年7月發行包含下列功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>請注意，根據您目前的套件，項目會以星號( ![（星號）](assets/yellow-star.png))可能需要購買值附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

**_每季發行_** 下列功能將於 **2020年7月31日**.

## 管理 {#administration}

* **[欄位管理中的「使用者」匯出](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**:管理員現在可以將選取欄位的所有「使用者」資產連結匯出為CSV檔案。 此增強功能可協助管理員與非管理員清除未使用的欄位。 此外，資產現在可以在新的瀏覽器標籤或視窗中開啟。

## Account-Based Marketing {#account-based-marketing}

![（星號）](assets/yellow-star.png)

* **更新帳戶設定檔的UI**:透過簡化步驟，在單一畫面中簡化「帳戶設定檔」中建立目標帳戶清單的程式。

<br> 

**_整季推出_**

下列功能屬於非季度週期，將在未來數月內發行。

* **Forms服務**:我們推出更強大的表單欄位語法驗證功能，並透過新的「登錄頁面安全網域」功能，封鎖常見的機器人模式。 封鎖機器人模式可以減少垃圾郵件表單提交次數，並改善資料庫品質。

>[!NOTE]
>
>增強表單欄位語法驗證的完整推出已延後至2021年1月版本之後。

* **增加資產API URI大小限制**:在刪除&quot;_method&quot;參數之前，統一資源標識符(URI)大小限制從8KB增加到65KB。 執行長查詢字串時，增加此大小限制可讓資料更輕鬆傳遞。 移除「_method」參數是即將進行之安全性升級的一部分。

## Sales Insight {#sales-insight}

![（星號）](assets/yellow-star.png)

* **[為具有非原生Salesforce CRM整合的客戶啟用Sales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) （測試版）**:具有非原生Salesforce CRM整合的Marketo Engage客戶現在可以使用Sales Insight來協助其銷售團隊了解、排定優先順序，並與參與最多的銷售機會互動，以實現智慧銷售和更快的交易。

## Sales Connect {#sales-connect}

![（星號）](assets/yellow-star.png)

* **[增強銷售呼叫的雙方同意：](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** 現在，管理員對呼叫記錄設定擁有更大的控制權。 [啟用呼叫錄制](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) 信心地遵守雙方同意法。 自動記錄呼叫的通知，並啟動要在呼叫之前播放的音訊剪輯。

<br> 

## 公告與淘汰 {#announcements-deprecations}

* **移除資產API「_method」參數**:2020年9月後，資產API端點將不再接受「_method」在POST內文中傳遞查詢參數，以略過URI長度限制。 為符合需要此參數的要求，資產API的URI限制將從8KB增加到65KB。
* **[Munchkin關聯銷售線索](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:在Munchkin JavaScript用戶端159版的發行中，我們將開始淘汰Munchkin Associate Lead方法。 如果叫用，您會收到警告，指出該方法將在未來版本中移除。 移除後，方法將無法繼續運作，且嘗試使用方法將會失敗。 Marketo Engage客戶若最近使用此方法，將會收到個別使用通知。
* **支援Internet Explorer**:如先前所宣佈，Internet Explorer 11的Marketo Engage支援將於 **2020年7月31日**. 我們將繼續支援Google Chrome、Mozilla Firefox、Apple Safari和Microsoft Edge。
* **天空預設體驗**:此版本將移除管理員或使用者將Marketo Sky設為預設體驗的選項，以準備更新至主要使用者體驗。 有關更新主要體驗的更多詳細資訊將於今年晚些時候推出，將於7月推出。 將Marketo Sky設為預設體驗或已獲得Marketo Sky存取權的使用者，可以繼續從「我的Marketo」首頁的圖磚存取Marketo Sky。
* **EdgeHTML（非Chromium）Microsoft Edge支援**:2020年底，Marketo Engage將不再支援Microsoft Edge的EdgeHTML版本。 自2021年1月1日起，我們將僅支援最新的Chromium版Microsoft Edge。
