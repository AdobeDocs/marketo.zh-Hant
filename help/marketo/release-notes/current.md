---
description: 當前發行說明 — Marketo文檔 — 產品文檔
title: 當前發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: e489ab3e5e4f1d6628db525e53207d229b50a92b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 發行說明：2022年5月 {#release-notes-may-22}

在下面，您將找到2022年5月版本中包含的所有功能。 檢查您的AdobeMarketo Engage版以瞭解功能可用性。

>[!AVAILABILITY]
>
>用星表示的特徵(![星](assets/yellow-star.png))是付費附加項。 請聯繫您的Marketo Engage代表以瞭解詳細資訊。

**_季度發佈_**

以下功能將開始在 **2022年5月6日**，在隨後的幾週內分階段部署剩餘功能（除非另有說明）。

## 本機CRM整合 {#native-crm-integration}

**[本機Veeva CRM整合](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target=&quot;_blank&quot;}（可用性有限）**:通過本機整合在Veeva CRM和Marketo Engage之間同步活動，改善與醫療保健專業人員的接觸。 這一整合使營銷人員能夠為醫療保健專業人員創造更個性化和無縫的跨渠道體驗。 如果您有興趣參與，請與您的客戶成功經理聯繫。

## 跨通道業務流程 {#cross-channel-orchestration}

**動態聊天的Chatbot事件**:利用Web訪問者更詳細的行為資料，如頁上時間、站點時間和頁面滾動百分比，以定義何時應顯示聊天對話框。

**PDF嵌入用於動態聊天**:通過將PDF嵌入聊天對話中來增加參與並共用有意義的內容，並通過參與活動跟蹤來衡量內容效能。

**動態聊天的擴展語言支援**:現在，動態聊天用戶介面也將以法語、德語、日語、葡萄牙語和西班牙語提供。 還可以用這些語言配置聊天對話框。

**排除動態聊天的URL**:控制「動態聊天」顯示的網頁中哪些網頁，能夠將特定URL排除在目標條件之外。

**[電子郵件Bot活動篩選增強](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target=&quot;_blank&quot;**:除現有IAB清單匹配標識外，還能夠根據隱藏的連結用戶代理或IP和鄰近模式來標識bot行為，從而繼續保護資料庫的健康。 查看允許您瞭解每種類型所標識的bot活動數的bot活動統計。

**[電子郵件跟蹤連結的STS標題](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target=&quot;_blank&quot;**:通過應用安全傳輸安全報頭來確保跟蹤鏈路的通信始終安全，來滿足安全最佳實踐。

## 新一代體驗 {#next-generation-experience}

**切換預設為新一代體驗的交換機**：切換開關將預設為所有可用螢幕中的新體驗，使用戶更容易發現更新的設計和可用性增強。

**新一代體驗中的更新螢幕**:

我們將在Design Studio中提供新一代體驗的電子郵件模板詳細資訊視圖，提供可通過切換開關訪問的更新的設計和可用性增強功能。

## 體驗自動化 {#experience-automation}

**自助流程步驟（續beta）**:通過編寫自定義流步驟以便在智慧市場活動中使用，擴展Marketo Engage與堆棧其餘部分之間的連接。 Marketo Engage用戶和合作夥伴都可以利用此功能允許在觸發、批處理和可執行市場活動中使用外部Web服務（與只能在觸發市場活動中使用的Webhook不同）。

## API增強 {#api-enhancements}

* **已擴展的API訪問權限，用於啟用CRM的訂閱**:我們正在擴展對啟用了CRM同步的訂閱的API訪問，以允許用戶從Marketo Engage中檢索公司、機會和銷售人員。
* **支援Forms的「隱藏」資料類型**:提供通過API管理隱藏表單域的功能。
* **通過規則支援isNot窗體的多個比較值**:根據另一個欄位的值是否不是給定清單中的值之一，管理表單欄位的可見性。
* **允許在「單獨選擇清單」中設定顯示值和已提交值**:在欄位中分別設定顯示值和提交值。 例如，顯示酒店名稱，但向後端提交內部ID。
* **允許在建立或更新電子郵件時禁用開啟跟蹤**:建立禁用開啟跟蹤的電子郵件。

## 公告 {#announcements}

**電子郵件驗證和唯一性**:從4月開始，電子郵件驗證將開始實施。 此時，Marketo Engage用戶電子郵件地址將需要驗證和唯一性（這不適用於僅API用戶）。 當使用「電子郵件驗證」啟用訂閱時，經目錄服務驗證的用戶將自動驗證其電子郵件。

使用「登錄邀請用戶對話框」功能或具有與多個用戶關聯的單個電子郵件的訂閱的電子郵件驗證將與五月份的版本一致。 與多個用戶關聯的單個電子郵件的訂閱將啟用「電子郵件驗證」，並將要求這些用戶解決衝突並為每個用戶使用唯一的電子郵件。 啟用「登錄邀請用戶對話框」功能後，通過此功能邀請的用戶將需要具有唯一的電子郵件地址。 對於通過此功能邀請的僅API用戶，電子郵件地址不必唯一。

**存檔資料夾行為更改**:在此版本中，在「存檔」資料夾中建立新資產的功能將不再可以從樹上下文菜單中獲得。 用於建立新資產的菜單選項將隱藏於所有資產中。 [在此處瞭解更多資訊](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target=&quot;_blank&quot;}。

**_產品發佈網路研討會_**

2022年5月11日，上午9:00 PT /下午12:00 PM, [即時網路研討會](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html)由我們的產品團隊托管的{target=&quot;_blank&quot;}，您可以在其中學習如何使用所有最新的產品創新。
