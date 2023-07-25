---
description: 發行說明 — 2022年1月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2022年1月
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 發行說明： 2022年1月 {#release-notes-jan-22}

2022年1月發行版本包含下列功能。 檢視您的Adobe Marketo Engage版本，瞭解是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![星號](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

下列功能將開始發行： **2022年1月21日**，並在接下來的幾週內分階段推出每個功能（除非另有指定）。

## 新一代體驗 {#modern-ux}

* **更新下一代體驗的畫面**：我們將在新一代體驗中提供額外的重新整理畫面，透過切換開關提供更新的設計和可用性增強功能：

   * Design Studio中的登陸頁面資產詳細資訊
   * 行銷活動中的登陸頁面資產詳細資訊

## Microsoft Dynamics整合 {#microsoft-dynamics-integration}

* **同步多重選取選項集欄位型別一般可用**：同步處理Microsoft Dynamics中的多選選項集欄位型別，以便在智慧列示和智慧行銷活動中運用，以獲得更精細的對象目標定位。 範例包括：相關主題/產品、偏好的通訊模式等。 此新同步處理適用於Microsoft Dynamics 9.X版（包括Dynamics 365 Online）。

* **適用於Microsoft Dynamics 365 Online的伺服器對伺服器驗證**：為了提高安全性，我們現在將支援伺服器對伺服器(S2S)，作為Azure Active Directory上Marketo Engage同步處理使用者的額外驗證模式，以進行非互動式存取Microsoft Dynamics 365 Online。 這可讓您採用多重驗證，因為所有驗證和登入都將以OAuth （只有使用者端ID和使用者端密碼）為基礎。

>[!NOTE]
>
>S2S模式是以「應用程式使用者」而非「授權使用者」為基礎，因此可節省使用額外的授權。

## 管理 {#administration}

* **[表單驗證規則](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**：維護資料庫的健全狀態，並有能力封鎖有問題或不需要的電子郵件網域提交Marketo Engage表單。 「全域表單驗證規則」面板可讓管理員定義封鎖清單，或啟用預先定義的自由消費者網域清單，以封鎖表單。

* **[登陸頁面頁首安全性](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**：管理員可以管理其登陸頁面網域上的嚴格傳輸安全性和X-Frame Options標頭，以強制執行嚴格的安全性要求。

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## AEPMarketo Engage目的地聯結器 — 建立全新銷售機會 {#aep-marketo-engage-destination-connector}

同時使用Adobe Experience Platform (AEP)的Marketo Engage客戶可透過AEP目的地聯結器，將全新個人記錄從AEP推送到Marketo Engage，將資料庫最大化。 將受眾區段從AEP傳送至Marketo Engage時，區段內尚未存在於Marketo Engage資料庫中的人員 [可自動新增至其中](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## 銷售分析 {#sales-insight}

![（星號）](assets/yellow-star.png)

**Salesforce CRM的銷售分析**

* **最適化的新型別欄**：賣家將透過標籤為「型別」的新欄位更快獲得深入分析，以區分「最佳選擇」頁面上的潛在客戶與聯絡人。

* **Salesforce平台API更新**：為因應Salesforce淘汰Salesforce平台API 21.0到30.0版，已更新Sales Insight套件，其中包含最新的API。

* **更新的品牌**：正在更新所有Sales Insight頁面，以符合Adobe品牌。

**Microsoft Dynamics的銷售分析**

* **已更新帳戶配置**：賣家可獲得熱門活動的整體檢視，例如：電子郵件活動、網路活動、有趣的時刻，以及帳戶內所有聯絡人的分數變更。

## Sales Connect {#sales-connect}

![（星號）](assets/yellow-star.png)

* **通話結果和原因**：透過全新、完全自訂的來電結果和來電原因選項，更詳細地瞭解及追蹤您的銷售團隊的對外付出。 除了這些新欄位外，我們還將推出新的控管功能，在銷售者打電話時強制來電理由和結果選擇，並推出新的控管功能，以啟用或停用來電理由和結果，以及新的來電理由和來電結果Salesforce活動自訂欄位，用於將資料記錄到Salesforce。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) 以深入瞭解。

* **Salesforce活動詳細資料自訂**：當銷售活動從Sales Connect登入Salesforce時，透過自訂要新增到Salesforce任務主題欄位的資訊，擷取更多Salesforce活動和任務資料。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) 以深入瞭解。

## 公告 {#announcements}

* **Marketo Sky淘汰**：三月起，我們將資源聚焦於提供新一代的使用者體驗，因此將不再提供Marketo Sky。 為了維持對當今Marketo Sky專屬功能的存取，我們在3月將資產到期和智慧行銷活動優先順序覆寫納入主流體驗。 [按一下這裡](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) 以深入瞭解。

* **表單端點淘汰**：Marketo Engage表單會拒絕不支援程式化表單的leadCapture/save2端點POST。 [按一下這裡](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) 以深入瞭解。

**Marketo Engage網域 — Sales Insight設定**：對於未布建SSL憑證和https://的Marketo Engage網域，呼叫將失敗並出現SSL交握錯誤。 因此，這些網域將會淘汰。 因此，使用指向這些網域中任何網域之舊設定的Sales Insight使用者，可能會在其Lead、Contact、Account、Opportunity Panels或Marketo Global頁面上遇到系統圖說文字錯誤。 建議您更新 [Marketo Engage設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) Salesforce中（如果您遇到此錯誤）。 您只需要更新檔案中「Marketo銷售分析設定」區段中醒目提示的Marketo Engage認證。

**_產品發行網路研討會_**

[2022年1月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
