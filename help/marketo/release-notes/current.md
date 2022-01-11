---
description: 最新發行說明 — Marketo檔案 — 產品檔案
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 534fb9d253b84147fe7fc96ce15987318dcea882
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# 發行說明：2022年1月 {#release-notes-jan-22}

』22年1月發行版本包含下列功能。 查看您的AdobeMarketo Engage版，了解功能是否可用。

>[!AVAILABILITY]
>
>以星號表示的特徵(![星星](assets/yellow-star.png))是付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

**_每季發行_**

下列功能將於 **2022年1月21日**.

## 新一代體驗 {#next-generation-experience}

* **新一代體驗中的更新畫面**:我們在新一代體驗中提供更多經過更新的畫面，提供可透過切換開關存取的更新設計和可用性增強功能：

   * Design Studio中的登錄頁面資產詳細資訊
   * 行銷活動中的登陸頁面資產詳細資料

## Microsoft Dynamics整合 {#microsoft-dynamics-integration}

* **同步多選選項集欄位類型通常可用**:從Microsoft Dynamics同步多選選項集欄位類型，以在智慧清單和智慧促銷活動中運用，以鎖定更精細的對象。 範例包括：感興趣的主題/產品、偏好的通訊模式等。 此新同步功能適用於Microsoft Dynamics 9.X版（包括Dynamics 365 Online）。

* **Microsoft Dynamics 365 Online的伺服器對伺服器驗證**:為了提高安全性，我們現在將支援伺服器對伺服器(S2S)，作為Azure Active Directory上Marketo Engage同步用戶的額外身份驗證模式，以非互動式訪問Microsoft Dynamics 365 Online。 這可讓您採用多重驗證，因為所有驗證和登入都將以OAuth為基礎（僅限用戶端ID和用戶端密碼）。

>[!NOTE]
>
>S2S模式以應用程式用戶（而非授權用戶）為基礎，這樣可節省額外許可證的使用。

## 管理 {#administration}

* **表單驗證規則**:維護資料庫的運行狀況，並能夠阻止有問題或不需要的電子郵件域提交Marketo Engage表。 「全域表單驗證規則」面板可讓管理員定義封鎖清單，或啟用預先定義的自由消費者網域清單，以封鎖表單。

* **登錄頁面標題安全性**:管理員可以在其登陸頁面網域上管理嚴格的傳輸安全性和X-Frame選項標題，以強制執行強大的安全性要求。

**_整季推出_**

下列功能屬於非季度週期，將在未來數月內發行。

## AEPMarketo Engage目的地連接器 — 建立新銷售機會 {#aep-marketo-engage-destination-connector}

同時使用Adobe Experience Platform(AEP)的Marketo Engage可透過AEP目的地連接器，將新人員記錄從AEP推送至Marketo Engage，進而將其資料庫發揮到最大。 將受眾區段從AEP傳送至Marketo Engage時，區段內尚未存在於Marketo Engage資料庫中的人員會自動新增至區段。

## Sales Insight {#sales-insight}

![（星號）](assets/yellow-star.png)

**Salesforce CRM的Sales Insight**

* **新類型欄以獲得最佳結果**:賣家將能透過標示為「類型」的新欄，更快速地獲得深入分析，以區分「最佳下注」頁面上的銷售機會和聯絡人。

* **Salesforce平台API更新**:為因應Salesforce淘汰的Salesforce Platform API 21.0版到30.0版，Sales Insight套件已使用最新API更新。

* **更新品牌**:所有Sales Insight頁面都會更新，以與Adobe品牌一致。

**Microsoft Dynamics的Sales Insight**

* **更新帳戶配置**:銷售者可以取得最熱門活動的集體檢視，例如：帳戶內所有連絡人的電子郵件活動、網路活動、有趣時刻和分數變更。

## Sales Connect {#sales-connect}

![（星號）](assets/yellow-star.png)

* **呼叫結果和理由**:使用全新、可完全自定義的呼叫結果和呼叫原因選項，更詳細地了解和跟蹤銷售團隊的出站工作。 除了這些新欄位，我們還推出新的管理，以在銷售商進行呼叫時強制執行呼叫原因和結果選擇，啟用或停用呼叫原因和結果的新管理，以及新的「呼叫原因」和「呼叫結果Salesforce活動」自訂欄位，用於將資料記錄到Salesforce。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) 了解更多。

* **Salesforce活動詳細資訊定制**:當銷售活動從Sales Connect記錄到Salesforce時，通過自定義添加到Salesforce任務主題欄位的資訊，在Salesforce中捕獲更多銷售活動和任務資料。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) 了解更多。

## 公告 {#announcements}

* **Marketo Sky日落設定**:3月11日起，我們將不再提供Marketo Sky，因為我們將資源集中於提供新一代的使用者體驗。 為了持續存取目前Marketo Sky所獨有的功能，我們將於3月將資產過期和智慧型促銷活動優先順序覆寫納入主流體驗。

* **不再使用表單端點**:不支援的程式化表單POST到leadCapture/save2端點將被Marketo Engage表單拒絕。 [按一下這裡](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) 了解更多。

* **電子郵件驗證**:自此版本後，Marketo Engage訂閱將開始有「僅限非API」使用者驗證電子郵件地址。 通過電子郵件驗證啟用訂閱時，已驗證的目錄服務用戶將自動驗證其電子郵件。 使用「在邀請使用者對話方塊中登入」功能的使用者，或訂閱者若訂閱中有與多位使用者相關聯的單一電子郵件，將會延遲電子郵件驗證，並與3月終止此功能的時間一致。

* **在「邀請用戶」對話框中登錄**:3月時，將不再使用現有的「在邀請使用者對話方塊中登入」選用功能。 「在邀請使用者對話方塊中登入」功能遭到通用ID功能覆寫，這是即將推出的Identity Management系統整合所需的功能，已於2021年8月在所有訂閱上啟用。 經過淘汰後，Marketo Engage只會強制一個使用者與訂閱內的每個電子郵件地址相關聯。

**Marketo Engage網域 — Sales Insight設定**:對於未布建SSL憑證和https://的Marketo Engage網域，呼叫會失敗並出現SSL交握錯誤。 因此，這些領域將被淘汰。 因此，如果Sales Insight使用者的配置較舊，指向其中任何一個網域，則其銷售機會、聯繫人、帳戶、銷售機會面板或Marketo全域頁面可能會遇到系統註解錯誤。 建議您更新 [Marketo Engage配置](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) 在Salesforce中遇到此錯誤。 您只需更新檔案「Marketo Sales Insight Config」區段中強調顯示的Marketo Engage憑證。
