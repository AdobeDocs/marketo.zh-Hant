---
unique-page-id: 45416698
description: 發行說明–2020年7月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2020年7月
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 2%

---

# 發行說明：2020 年 7 月 {#release-notes-july}

2020年7月發行版本包含下列功能。 檢查您的Marketo版本是否有功能可用。

>[!AVAILABILITY]
>
>請注意，根據您目前的套件，含星號( ![（星號）](assets/yellow-star.png))的專案可能需要購買附加值。 請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

**_每季發行_**&#x200B;下列功能將於2020年7月31日&#x200B;**發行**。

## 管理 {#administration}

* 欄位管理中的&#x200B;**[「使用者」匯出](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**：管理員現在可以將所選欄位的所有「使用者」資產連結匯出至CSV檔案。 此增強功能可協助管理員與非管理員清除未使用的欄位。 此外，資產現在可以在新的瀏覽器標籤或視窗中開啟。

## Account-Based Marketing {#account-based-marketing}

![（星形）](assets/yellow-star.png)

* **已更新帳戶設定檔的UI**：簡化在帳戶設定檔中建立目標帳戶清單的步驟，所有步驟都可在單一畫面中完成。

<br>

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

* **Forms服務**：我們將推出更強大的表單欄位語法驗證，以及封鎖具有登陸頁面功能之新安全網域的一般機器人模式的功能。 封鎖機器人模式可以減少垃圾郵件表單提交並改善資料庫品質。

>[!NOTE]
>
>增強型表單欄位語法驗證的完整推出已推遲到2021年1月發行版本之後。

* **增加資產API URI大小限制**：統一資源識別碼(URI)大小限制在移除「_method」引數之前，已從8KB增加到65KB。 執行長查詢字串時，此大小限制增加會讓資料更輕鬆地傳遞。 移除「_method」引數是即將進行的安全性升級的一部分。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

* **[[!DNL Sales Insight] 針對非原生客戶啟用 [!DNL Salesforce] CRM整合](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**：具有非原生[!DNL Salesforce] CRM整合的Marketo Engage客戶現在可以使用[!DNL Sales Insight]，協助其銷售團隊瞭解、排定優先順序並與參與度最高的銷售機會和機會互動，以實現聰明銷售和更快的交易。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **[銷售電話的增強型雙方同意：](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)**&#x200B;管理員現在對電話錄製設定有更大的控制權。 [啟用通話錄製](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md)，並確信您遵守雙方同意法。 自動通知正在錄製的通話，並啟動通話前要播放的音訊片段。

<br>

## 公告與淘汰 {#announcements-deprecations}

* **資產API「_method」引數移除**： 2020年9月後，資產API端點將不再接受於POST主體中使用「_method」傳遞查詢引數，以略過URI長度限制。 為因應需要此引數的請求，資產API的URI限制將從8KB增加到65KB。
* **[[!DNL Munchkin] 關聯銷售機會](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：在此版本的Munchkin JavaScript Client （版本159）中，我們將開始棄用[!DNL Munchkin] Associate Lead方法。 如果叫用，您將會收到警告，指出將在未來版本中移除方法。 移除後，方法將無法繼續運作，並且嘗試使用它將失敗。 最近使用過此方法的Marketo Engage客戶將會個別收到使用通知。
* **支援Internet Explorer**：如先前宣佈的，Marketo Engage對Internet Explorer 11的支援將於&#x200B;**2020年7月31日**&#x200B;結束。 我們將繼續支援[!DNL Google Chrome]、[!DNL Mozilla Firefox]、[!DNL  Apple Safari]和[!DNL Microsoft Edge]。
* **Sky預設體驗**：管理員或使用者將[!DNL Marketo Sky]設定為預設體驗的選項將在此版本中移除，以準備更新主要使用者體驗。 主要體驗更新的更多詳細資訊預計在今年晚些時候推出，將於7月推出。 已將[!DNL Marketo Sky]設定為其預設體驗，或已授與[!DNL Marketo Sky]存取許可權的使用者，可以繼續從「我的Marketo」首頁上的圖磚存取[!DNL Marketo Sky]。
* **支援EdgeHTML （非Chromium） [!DNL Microsoft Edge]**： 2020年底Marketo Engage將不再支援Microsoft Edge的EdgeHTML版本。 自2021年1月1日起，我們將僅支援最新的Microsoft Edge Chromium版本。
