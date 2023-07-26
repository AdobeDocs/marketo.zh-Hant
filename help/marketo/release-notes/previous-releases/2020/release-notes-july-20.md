---
unique-page-id: 45416698
description: 發行說明–2020年7月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年7月
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# 發行說明： 2020年7月 {#release-notes-july}

2020年7月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

>[!AVAILABILITY]
>
>請注意，根據您目前的封裝，專案會以星號( ![（星形）](assets/yellow-star.png))可能需要購買附加價值。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_** 下列功能將會發行於 **2020年7月31日**.

## 管理 {#administration}

* **[欄位管理中的「使用者」匯出](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**：管理員現在可以將所選欄位的所有「使用者」資產連結匯出至CSV檔案。 此增強功能可協助管理員與非管理員清除未使用的欄位。 此外，資產現在可以在新的瀏覽器標籤或視窗中開啟。

## Account-Based Marketing {#account-based-marketing}

![（星形）](assets/yellow-star.png)

* **已更新帳戶分析的UI**：透過簡化步驟（所有這些都在單一畫面中），簡化在帳戶設定檔中建立目標帳戶清單的過程。

<br> 

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

* **Forms服務**：我們將推出更強大的表單欄位語法驗證，且能夠使用登陸頁面功能的新安全網域封鎖常見的機器人模式。 封鎖機器人模式可以減少垃圾郵件表單提交並改善資料庫品質。

>[!NOTE]
>
>增強型表單欄位語法驗證的完整推出已推遲到2021年1月發行版本之後。

* **增加資產API URI大小限制**：統一資源識別碼(URI)大小限制在移除「_method」引數前已從8KB增加到65KB。 執行長查詢字串時，此大小限制增加會讓資料更輕鬆地傳遞。 移除「_method」引數是即將進行的安全性升級的一部分。

## 銷售分析 {#sales-insight}

![（星形）](assets/yellow-star.png)

* **[為具有非原生Salesforce CRM整合的客戶啟用Sales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**：透過非原生Salesforce CRM整合的Marketo Engage客戶，現在可以使用Sales Insight來協助其銷售團隊瞭解、安排優先順序並與最積極的潛在客戶及機會互動，以實現聰明銷售和更快的交易。

## Sales Connect {#sales-connect}

![（星形）](assets/yellow-star.png)

* **[增強銷售電話的雙方同意：](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** 管理員現在對通話錄製設定有更大的控制權。 [啟用通話錄製](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) 確信您遵守了雙方同意法。 自動通知正在錄製的通話，並啟動通話前要播放的音訊片段。

<br> 

## 公告與淘汰 {#announcements-deprecations}

* **資產API「_method」引數移除**：在2020年9月之後，資產API端點將不再接受於POST主體中使用「_method」傳遞查詢引數，以略過URI長度限制。 為因應需要此引數的請求，資產API的URI限制將從8KB增加到65KB。
* **[Munchkin關聯銷售機會](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：在此版本的Munchkin JavaScript Client 159中，我們將開始淘汰Munchkin Associate Lead方法。 如果叫用，您將會收到警告，指出將在未來版本中移除方法。 移除後，方法將無法繼續運作，並且嘗試使用它將失敗。 最近使用過此方法的Marketo Engage客戶將會個別收到使用通知。
* **支援Internet Explorer**：如先前宣佈的，Marketo Engage對Internet Explorer 11的支援結束於 **2020年7月31日**. 我們將繼續支援Google Chrome、Mozilla Firefox、Apple Safari和Microsoft Edge。
* **Sky預設體驗**：管理員或使用者將Marketo Sky設定為預設體驗的選項將在此版本中移除，以準備主要使用者體驗的更新。 主要體驗更新的更多詳細資訊預計在今年晚些時候推出，將於7月推出。 已將Marketo Sky設定為其預設體驗，或已獲得Marketo Sky存取許可權的使用者，可以繼續從「我的Marketo」首頁上的圖磚存取Marketo Sky。
* **EdgeHTML （非Chromium） Microsoft Edge支援**：2020年底，Marketo Engage將不再支援Microsoft Edge的EdgeHTML版本。 自2021年1月1日起，我們將僅支援最新的Microsoft Edge Chromium版本。
