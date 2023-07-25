---
description: 發行說明 — 2022年5月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2022年5月
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# 發行說明： 2022年5月 {#release-notes-may-22}

下方提供2022年5月發行版本包含的所有功能。 檢視您的Adobe Marketo Engage版本，瞭解是否有功能可用。

>[!AVAILABILITY]
>
>以星號(![星號](assets/yellow-star.png))為付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

下列功能將開始發行： **2022年5月6日**，在接下來的幾週內分階段推出剩餘的功能（除非另有指定）。

## 原生CRM整合 {#native-crm-integration}

**[原生Veeva CRM整合](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} （可用性限制）**：透過原生整合，在Veeva CRM和Marketo Engage之間同步活動，藉此改善與醫療保健專業人員的互動。 此整合可讓行銷人員為醫療保健專業人員建立更個人化且順暢的跨管道體驗。 如果您有興趣參與，請聯絡Adobe客戶團隊（您的客戶經理）。

## 跨頻道協調 {#cross-channel-orchestration}

**適用於Dynamic Chat的聊天機器人事件**：利用網頁訪客的更詳細行為資料，例如頁面逗留時間、網站逗留時間和頁面捲動百分比，以定義應何時顯示聊天對話方塊。

**PDF內嵌以進行Dynamic Chat**：將PDF內嵌到聊天對話方塊中，並透過參與活動追蹤來測量內容效能，藉此提高參與度並分享有意義的內容。

**Dynamic Chat的延伸語言支援**：Dynamic Chat使用者介面現在也將提供法文、德文、日文、葡萄牙文和西班牙文版本。 也可以用這些語言設定聊天對話方塊。

**排除Dynamic Chat的URL**：控制您的網頁Dynamic Chat會顯示在哪一個上，並有能力從鎖定目標條件中排除特定URL。

**[電子郵件機器人活動篩選增強功能](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**：除了現有的IAB清單比對識別之外，還能根據隱藏的連結「使用者代理」或IP和近似程度模式來識別機器人行為，繼續保護資料庫的健全狀態。 檢視機器人活動統計資料，以瞭解每種型別識別的機器人活動數目。

**[電子郵件追蹤連結的STS標題](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**：套用Secure Transport Security標頭的功能符合安全性最佳實務，以確保追蹤連結的流量一律安全。

## 新一代體驗 {#modern-ux}

**切換切換切換器預設為新一代體驗**：切換開關將在所有可用熒幕中預設為新體驗，讓使用者更容易發現更新的設計和可用性增強功能。

**更新畫面，提供新一代的體驗**：

我們在Design Studio中提供新一代體驗中的電子郵件範本詳細資料檢視，提供更新的設計和可用性增強功能，可透過切換開關存取。

## 體驗自動化 {#experience-automation}

**自助服務流程步驟（續測試版）**：藉由撰寫自訂的流程步驟以用於Smart Campaigns的功能，擴展Marketo Engage與棧疊其餘部分之間的連線。 Marketo Engage使用者和合作夥伴均可運用此功能，允許在觸發程式、批次和可執行的行銷活動中使用外部Web服務（與只能在觸發式行銷活動中使用的Webhook不同）。

## API增強功能 {#api-enhancements}

* **擴充CRM啟用訂閱的API存取權**：我們擴展已啟用CRM同步之訂閱的API存取權，讓使用者能從Marketo Engage中擷取公司、商機和銷售人員。
* **支援Forms中的「隱藏」資料型別**：提供透過API管理隱藏表單欄位的功能。
* **支援isNot Form透過規則的多重比較值**：根據其他欄位的值是否不是給定清單中的值之一來管理表單欄位的可見性。
* **允許分別設定選取清單中的顯示值和提交值**：在欄位中分別設定顯示值和提交值。 例如，顯示飯店的名稱，但向後端提交內部ID。
* **允許設定在建立或更新電子郵件時停用開啟追蹤**：建立停用開啟追蹤的電子郵件。

## 公告 {#announcements}

**電子郵件驗證和唯一性**：從4月開始，電子郵件驗證將開始推出。 屆時，Marketo Engage使用者電子郵件地址將需要驗證和唯一性（這不適用於僅API使用者）。 目錄服務驗證的使用者會在訂閱啟用電子郵件驗證時，自動驗證其電子郵件。

使用「在邀請使用者對話方塊中登入」功能或擁有與多位使用者相關聯之單一電子郵件的訂閱電子郵件驗證，將與5月版本一致。 若訂閱擁有與多位使用者相關聯的單一電子郵件，將會啟用電子郵件驗證，並將要求這些使用者解決衝突並使用每位使用者的唯一電子郵件。 啟用「在邀請使用者對話方塊中登入」功能時，透過此功能受邀的使用者將需要唯一的電子郵件地址。 對於透過此功能邀請的僅API使用者，電子郵件地址不需要是唯一的。

**封存資料夾行為變更**：在此版本中，樹狀結構快顯選單將不再提供在封存資料夾中建立新資產的功能。 所有資產都會隱藏用來建立新資產的功能表選項。 [在此處瞭解更多](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_產品發行網路研討會_**

[2022年3月和5月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
