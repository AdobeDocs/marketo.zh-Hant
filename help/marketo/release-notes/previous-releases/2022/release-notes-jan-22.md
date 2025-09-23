---
description: 發行說明 — 2022年1月 — Marketo檔案 — 產品檔案
title: 發行說明 - 2022 年 1 月
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 4%

---

# 發行說明：2022 年 1 月 {#release-notes-jan-22}

2022年1月發行版本包含下列功能。 請查看您的 Adobe Marketo Engage 版本是否提供這些功能。

>[!AVAILABILITY]
>
>標有星號 (![星號](assets/yellow-star.png)) 的功能為付費附加元件。請聯絡您的 Marketo Engage 代表，了解更多相關資訊。

**_每季發行_**

下列功能將於&#x200B;**2022年1月21日**&#x200B;開始發行，並在接下來的幾週內分階段推出每個功能（除非另有指定）。

## 次世代體驗 {#modern-ux}

* **新一代體驗中的Screens已更新**：我們為新一代體驗提供額外的重新整理熒幕，透過切換開關提供更新的設計和可用性增強功能：

   * 在[!UICONTROL Design Studio]中的登陸頁面資產詳細資訊
   * 在[!UICONTROL Marketing Activities]中的登陸頁面資產詳細資訊

## [!DNL Microsoft Dynamics]整合 {#microsoft-dynamics-integration}

* **同步多重選取選項集欄位型別一般可使用**：同步處理來自[!DNL Microsoft Dynamics]的多重選取選項集欄位型別，以便在智慧列示和智慧行銷活動中運用，以更精細地鎖定受眾。 例如：相關主題/產品、偏好的通訊模式等。 此新同步處理適用於[!DNL Microsoft Dynamics] 9.X版（包括Dynamics 365 Online）。

* **[!DNL Microsoft Dynamics 365 Online]**&#x200B;的伺服器對伺服器驗證：為了提高安全性，我們現在將支援伺服器對伺服器(S2S)，作為Azure Active Directory上Marketo Engage同步處理使用者的額外驗證模式，以非互動式存取[!DNL Microsoft Dynamics 365 Online]。 這可讓您採用多重驗證，因為所有驗證和登入都將以OAuth為基礎（只有使用者端ID和使用者端密碼）。

>[!NOTE]
>
>S2S模式是以「應用程式使用者」而非「授權使用者」為基礎，因此可節省額外授權的使用。

## 管理 {#administration}

* **[表單驗證規則](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**：維護資料庫的健全狀態，能夠封鎖有問題或不需要的電子郵件網域不提交Marketo Engage表單。 「全域表單驗證規則」面板可讓管理員定義封鎖清單，或啟用預先定義的免費消費者網域清單，以封鎖表單。

* **[登陸頁面標頭安全性](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**：管理員可以管理其登陸頁面網域上的嚴格傳輸安全性和X-Frame Options標頭，以強制執行強大的安全性要求。

**_整個季度發行_**

下列功能採用非季度週期，並將在未來幾個月發行。

## AEP Marketo Engage目的地聯結器 — 建立全新銷售機會 {#aep-marketo-engage-destination-connector}

同時使用Adobe Experience Platform (AEP)的Marketo Engage客戶可透過Marketo Engage目的地聯結器，將全新人員記錄從AEP推送至AEP，讓資料庫發揮最大效用。 從AEP傳送對象區段至Marketo Engage時，區段內尚未存在於Marketo Engage資料庫[中的人員可自動新增至該資料庫](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

**[!DNL Sales Insight]CRM[!DNL Salesforce]的**

* **適用於[!UICONTROL Best Bets]**&#x200B;的新型別欄：賣家將透過標籤為「型別」的新欄取得更快的深入分析，以區分[!UICONTROL Best Bets]頁面上的潛在客戶與聯絡人。

* **[!DNL Salesforce]Platform API更新**：為回應[!DNL Salesforce]淘汰[!DNL Salesforce] Platform API 21.0到30.0版，[!DNL Sales Insight]套件已更新為最新的API。

* **已更新品牌**：正在更新所有[!DNL Sales Insight]頁面，以符合Adobe品牌。

**[!DNL Sales Insight]的[!DNL Microsoft Dynamics]**

* **已更新帳戶配置**：賣家可取得熱門活動的集體檢視，例如：電子郵件活動、網路活動、有趣的時刻，以及帳戶內所有連絡人的分數變更。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **通話結果和原因**：透過全新、完全可自訂的通話結果和通話原因選項，更詳細地瞭解及追蹤您的銷售團隊的出站工作。 除了這些新欄位之外，我們還將推出新的控管以強制進行來電原因和結果選擇、新的控管以啟用或停用來電原因和結果，以及新的來電原因和來電結果[!DNL Salesforce]活動自訂欄位，以將資料記錄到[!DNL Salesforce]。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812)瞭解更多資訊。

* **[!DNL Salesforce]活動詳細資料自訂**：當銷售活動從[!DNL Salesforce]登入[!DNL Salesforce]時，自訂要新增哪些資訊到[!DNL Salesforce]任務主題欄位，以在[!DNL Sales Connect]中擷取更多銷售活動和任務資料。 [按一下這裡](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819)瞭解更多資訊。

## 公告 {#announcements}

* **棄用Marketo Sky**：三月起，我們將不再提供Marketo Sky，因為我們的資源著重於提供新一代的使用者體驗。 為了維持對當今Marketo Sky專屬功能的存取權，我們在3月將資產到期和智慧型行銷活動優先順序覆寫帶入主流體驗。 [按一下這裡](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)瞭解更多資訊。

* **表單端點淘汰**：Marketo Engage表單將拒絕不支援的leadCapture/save2端點程式化表單POST。 [按一下這裡](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631)瞭解更多資訊。

* **在[邀請使用者]對話方塊中登入**： 3月起，將棄用現有的選擇性功能[在邀請使用者對話方塊中登入]。 即將推出的Adobe Identity Management系統整合需要通用ID功能，而此功能已在2021年8月對所有訂閱啟用「[!UICONTROL Login in Invite User Dialog]」功能。 淘汰後，Marketo Engage將僅強制訂閱內每個電子郵件地址關聯一名使用者。

**Marketo Engage網域 — [!DNL Sales Insight]設定**：對於未布建SSL憑證和https://的Marketo Engage網域，呼叫將失敗並出現SSL交握錯誤。 因此，這些網域將被淘汰。 因此，具有指向這些網域中任何網域之舊設定的[!DNL Sales Insight]使用者可能在其Lead、Contact、Account、Opportunity Panels或Marketo Global頁面上遇到系統圖說文字錯誤。 如果您發生這個錯誤，建議您在[更新](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)Marketo Engage設定[!DNL Salesforce]。 您只需要更新在檔案的「[!DNL Marketo Sales Insight]設定」區段中醒目提示的Marketo Engage認證。

**_產品發行網路研討會_**

[2022年1月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
