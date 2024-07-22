---
description: 發行說明 — 2022年5月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2022年5月
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# 發行說明： 2022年5月 {#release-notes-may-22}

以下是2022年5月發行版本包含的所有功能。 檢查您的Adobe Marketo Engage版本是否有功能可用。

>[!AVAILABILITY]
>
>以星號（![星號](assets/yellow-star.png)）表示的功能是付費附加元件。 請聯絡您的Marketo Engage代表以瞭解更多資訊。

**_每季發行_**

下列功能將於2022年5月6日&#x200B;**開始發行**，並在接下來的幾週內分階段推出剩餘功能（除非另有指定）。

## 原生CRM整合 {#native-crm-integration}

**[原生Veeva CRM整合](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} （可用性限制）**：透過原生整合，在Veeva CRM與Marketo Engage之間同步活動，以改善與醫療專業人員的互動。 此整合可讓行銷人員為醫療保健專業人員建立更個人化且順暢的跨管道體驗。 如果您有興趣參與，請聯絡Adobe客戶團隊（您的客戶經理）。

## 跨頻道協調 {#cross-channel-orchestration}

**Dynamic Chat的聊天機器人事件**：利用網頁訪客更詳細的行為資料，例如頁面逗留時間、網站逗留時間和頁面捲動百分比，以定義何時應顯示聊天對話方塊。

**Dynamic Chat的內嵌PDF**：將PDF內嵌到聊天對話方塊中，並透過參與活動追蹤來測量內容效能，藉此提高參與度和共用有意義的內容。

**Dynamic Chat的延伸語言支援**：Dynamic Chat使用者介面現在也將提供法文、德文、日文、葡萄牙文和西班牙文版本。 也可以用這些語言設定聊天對話方塊。

**排除Dynamic Chat的URL**：控制您的網頁Dynamic Chat出現在哪個網頁，並能夠從目標定位條件中排除特定URL。

**[電子郵件機器人活動篩選增強功能](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**：除了現有的IAB清單比對識別之外，還能根據隱藏連結使用者代理程式或IP和近似程度模式來識別機器人行為，繼續保護資料庫的健全狀態。 檢視機器人活動統計資料，以瞭解每種型別識別的機器人活動數目。

**[電子郵件追蹤連結的STS標頭](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**：符合安全性最佳實務，能夠套用Secure Transport Security標頭，以確保追蹤連結的流量一律安全。

## 次世代體驗 {#modern-ux}

**切換切換預設為新一代體驗**：切換切換切換將在所有可用熒幕中預設為新體驗，讓使用者更容易發現更新的設計和可用性增強功能。

**已更新下一代體驗中的畫面**：

我們在Design Studio中提供新一代體驗中的電子郵件範本詳細資料檢視，透過切換開關提供更新的設計和可用性增強功能。

## 體驗自動化 {#experience-automation}

**自助服務流程步驟（繼續測試版）**：擴充Marketo Engage與您棧疊其他部分之間的連線，並有能力編寫自訂流程步驟以用於Smart Campaigns。 Marketo Engage使用者和合作夥伴均可運用此功能，允許在觸發、批次和可執行的行銷活動中使用外部Web服務（相較於只能在觸發行銷活動中使用的Webhook）。

## API增強功能 {#api-enhancements}

* **已啟用CRM之訂閱的擴充API存取**：我們正在擴充已啟用CRM同步處理之訂閱的API存取，以允許使用者從Marketo Engage中擷取公司、商機和銷售人員。
* **在Forms中支援「隱藏」資料型別**：提供透過API管理隱藏表單欄位的功能。
* **透過Rules支援isNot表單的多重比較值**：根據其他欄位的值是否不是指定清單中的值之一來管理表單欄位的可見度。
* **允許分別設定選取清單中的顯示值和提交值**：分別設定欄位中的顯示值和提交值。 例如，顯示飯店的名稱，但將內部ID提交至後端。
* **允許在建立或更新電子郵件時停用開啟追蹤的設定**：建立已停用開啟追蹤的電子郵件。

## 公告 {#announcements}

**電子郵件驗證與唯一性**：從4月開始，將開始推出電子郵件驗證。 此時，Marketo Engage使用者電子郵件地址將需要驗證和唯一性（這不適用於僅限API的使用者）。 目錄服務已驗證的使用者會在訂閱啟用電子郵件驗證時，自動驗證其電子郵件。

使用「在邀請使用者對話方塊中登入」功能或擁有與多位使用者相關聯之單一電子郵件的訂閱電子郵件驗證，將與5月發行一致。 若訂閱擁有與多位使用者相關聯的單一電子郵件，則會啟用電子郵件驗證，並將要求這些使用者解決衝突並使用每位使用者的唯一電子郵件。 啟用「在邀請使用者對話方塊中登入」功能時，透過此功能受邀的使用者將需要唯一的電子郵件地址。 對於透過此功能邀請的僅API使用者，電子郵件地址不需要是唯一的。

**封存資料夾行為變更**：在此版本中，樹狀內容功能表中將不再提供在封存資料夾中建立新資產的功能。 將會為所有資產隱藏用來建立新資產的功能表選項。 [在這裡瞭解更多](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}。

**_產品發行網路研討會_**

[2022年3月和5月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
