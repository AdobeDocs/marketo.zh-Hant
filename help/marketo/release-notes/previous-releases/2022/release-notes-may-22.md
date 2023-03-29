---
description: 發行說明 — 2022年5月 — Marketo檔案 — 產品檔案
title: 發行說明 — 2022年5月
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# 發行說明：2022年5月 {#release-notes-may-22}

以下是』22年5月版本包含的所有功能。 查看您的Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號表示的特徵(![星星](assets/yellow-star.png))是付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

**_每季發行_**

下列功能將於 **2022年5月6日**，並在後續數週分階段推出剩餘功能（除非另有指定）。

## 原生CRM整合 {#native-crm-integration}

**[原生Veeva CRM整合](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} （可用性有限）**:透過原生整合將活動同步到Veva CRM與Marketo Engage之間，改善與醫療保健專業人員的互動。 此整合可讓行銷人員為醫療保健專業人員建立更個人化且順暢的跨管道體驗。 如果您有興趣參與，請連絡Adobe客戶團隊（您的客戶經理）。

## 跨管道協調 {#cross-channel-orchestration}

**用於動態聊天的聊天機器人事件**:運用網頁逗留時間、網站逗留時間和頁面捲動百分比等網站訪客的更詳細行為資料，以定義何時應顯示聊天對話方塊。

**PDF內嵌於動態聊天**:將PDF嵌入聊天對話方塊，並透過參與活動追蹤來測量內容效能，借此提高參與度並共用有意義的內容。

**Dynamic Chat的擴展語言支援**:現在，動態聊天使用者介面也提供法文、德文、日文、葡萄牙文和西班牙文版。 也可以使用這些語言配置聊天對話框。

**排除動態聊天的URL**:控制顯示哪些網頁動態聊天，並能將特定URL排除在目標定位條件之外。

**[電子郵件機器人活動篩選增強功能](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}**:除了現有的IAB清單比對識別外，還能根據隱藏的連結使用者代理或IP與鄰近地區模式，持續保護資料庫的健全狀態。 檢視機器人活動統計資料，以便您了解針對每種類型識別的機器人活動數量。

**[電子郵件追蹤連結的STS標題](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}**:符合安全性最佳實務，並能套用安全傳輸安全標頭，以確保對追蹤連結的流量一律安全。

## 新一代體驗 {#modern-ux}

**切換預設為新一代體驗**：切換開關將預設為所有可用畫面中的新體驗，讓使用者更容易探索更新的設計和可用性增強功能。

**新一代體驗中的更新畫面**:

我們提供新一代體驗中Design Studio中的電子郵件範本詳細資料檢視，提供可透過切換開關存取的更新設計和可用性增強功能。

## 體驗自動化 {#experience-automation}

**自助服務流程步驟（續測試版）**:借由編寫可在智慧行銷活動中使用的自訂流程步驟，擴展Marketo Engage與堆疊其餘部分之間的連線。 Marketo Engage使用者和合作夥伴都可運用此功能，在觸發、批次和可執行的促銷活動中使用外部Web服務（相較之下，WebHook只能用於觸發促銷活動）。

## API增強功能 {#api-enhancements}

* **針對啟用CRM的訂閱擴充API存取**:我們正在擴展訂閱的API存取權，這些訂閱已啟用CRM同步功能，讓使用者可從Marketo Engage中擷取公司、商機和銷售人員。
* **支援Forms中的「隱藏」資料類型**:提供透過API管理隱藏表單欄位的功能。
* **支援isNot透過規則的多個比較值**:根據另一個欄位的值是否不是指定清單中的值之一，管理表單欄位的可見性。
* **允許在選擇清單中單獨設定顯示值和已提交值**:在欄位中分別設定顯示值和已提交值。 例如，顯示酒店名稱，但將內部ID提交至後端。
* **允許在建立或更新電子郵件時禁用開啟跟蹤設定**:建立已停用開啟追蹤的電子郵件。

## 公告 {#announcements}

**電子郵件驗證與獨特性**:從4月開始，電子郵件驗證將開始推出。 此時，Marketo Engage使用者電子郵件地址將需要驗證和唯一性（這不適用於僅限API的使用者）。 通過電子郵件驗證啟用訂閱時，已驗證的目錄服務用戶將自動驗證其電子郵件。

使用「在邀請使用者對話方塊中登入」功能，或有單一電子郵件與多位使用者相關聯的訂閱，電子郵件驗證將會與5月發行版本一致。 若訂閱中有與多個使用者相關聯的單一電子郵件，將會啟用「電子郵件驗證」功能，並要求這些使用者解決衝突，並為每位使用者使用獨特的電子郵件。 啟用「在邀請使用者對話方塊中登入」功能時，透過此功能邀請的使用者將需要有唯一的電子郵件地址。 針對透過此功能邀請的僅限API使用者，電子郵件地址不需要唯一。

**封存資料夾行為變更**:在此版本中，樹狀內容功能表將不再提供在封存資料夾中建立新資產的功能。 用於建立新資產的功能表選項會針對所有資產而隱藏。 [如需詳細資訊，請前往這裡](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_產品發行網路研討會_**

[2022年3月和5月Marketo Engage發行網路研討會](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
