---
unique-page-id: 45416698
description: 發行說明- 2007年7月——行銷檔案——產品檔案
title: 發行說明- 2002年7月
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# 發行說明：20年7月 {#release-notes-july}

7月20日發行包含下列功能。 檢查您的Marketo版本，以取得功能。

>[!NOTE]
>
>**可用性**
>
>請注意，視您目前的套件而定，含星號( ![(star)](assets/star-yellow.svg))的項目可能需要購買附加值。 請連絡您的行銷人員以吸引客戶代表，以瞭解更多資訊。

***季度發行*** ：下列功能將於2020年7月31 **日發行**。

## 管理 {#administration}

* ** 「 [Used By」 Export in Field Management](https://docs.marketo.com/x/hAK1Ag)**:管理員現在可將選取欄位的所有「使用者」資產連結匯出為CSV檔案。 此增強功能可協助管理員和非管理員清除未使用的欄位。 此外，資產現在可以在新的瀏覽器標籤或視窗中開啟。

**帳戶型行銷 ![（星型）](assets/star-yellow.svg)

**

* **帳戶分析的更新UI:**透過單一畫面中簡化的步驟，簡化「帳戶分析」中目標帳戶清單的建立。

<br> 

**

***整季發行***

以下功能是非季度週期，將於未來數月內發佈。

* **表單服務：**我們推出更強大的表單欄位語法驗證，並運用新的著陸頁面安全網域功能來封鎖常見的機器人模式。 封鎖機器人模式可以減少垃圾郵件提交，並改善您的資料庫品質。
* **增加資產API URI大小限制**:在刪除&quot;_method&quot;參數之前，統一資源標識符(URI)大小限制從8KB增加到65KB。 執行長查詢字串時，此大小限制的增加可讓資料更容易傳遞。 移除&quot;_method&quot;參數是即將進行的安全性升級的一部份。

**Sales Insight ![（星型）](assets/star-yellow.svg)

**

* **針對 [非原生Salesforce CRM整合的客戶啟用銷售分析](https://docs.marketo.com/x/pQK1Ag)（測試版）**:行銷：透過非原生的Salesforce CRM整合，吸引客戶，現在可以使用Sales Insight來協助其銷售團隊瞭解、排定優先順序，並與最受吸引的客戶和機會互動，以實現智慧銷售和更快的交易。

**Sales Connect( ![星型)](assets/star-yellow.svg)

**

* **增 [強銷售電話的雙方同意：](https://docs.marketo.com/x/dgC1Ag)**管理員現在更能控制電話錄制設定。 [您可以放心地](https://docs.marketo.com/x/dAC1Ag) ，啟用通話錄制，確保您遵守雙方同意法。 自動記錄通話的通知，並啟用通話前要播放的音訊片段。

<br> 

## 公告與淘汰 {#announcements-deprecations}

* **資產API &quot;_method&quot;參數移除**:在2020年9月之後，資產API端點將不再接受&quot;_method&quot;來傳遞POST內文中的查詢參數，以略過URI長度限制。 為配合需要此參數的要求，資產API的URI限制將從8KB增加為65KB。
* ** [Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:在本版Munchkin JavaScript用戶端159版中，我們將開始淘汰Munchkin Associate Lead方法。 如果呼叫，您會收到警告，指出該方法將在未來版本中移除。 移除後，方法將不再正常運作，且嘗試使用方法將失敗。 Marketo Engage最近使用此方法的客戶將會收到個別使用的通知。
* **支援Internet Explorer**:如先前所宣佈，Marketo Engage對Internet Explorer 11的支援將於2020年7 **月31日截止**。 我們將繼續支援Google Chrome、Mozilla Firefox、Apple Safari和Microsoft Edge。

* **Sky預設體驗**:此版本將移除管理員或使用者將Marketo Sky設為預設體驗的選項，以備主要使用者體驗的更新。 預計在今年晚些時候推出的主要體驗更新的更多詳細資訊將於7月推出。 將Marketo Sky設為預設體驗，或已獲准存取Marketo Sky的使用者，可繼續從My Marketo首頁的方塊存取Marketo Sky。
* **EdgeHTML（非Chromium）Microsoft Edge支援**:Marketo Engage在2020年底將不再支援EdgeHTML版本的Microsoft Edge。 從2021年1月1日開始，我們將只支援最新版Chromium Edge。

