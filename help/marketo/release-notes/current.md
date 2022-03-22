---
description: 當前發行說明 — Marketo文檔 — 產品文檔
title: 當前發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: f2653a21eaa8c353afb0a1634a3301e3b6d5ab2d
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# 發行說明：2022年3月 {#release-notes-mar-22}

以下功能包含在2004年3月的發行版中。 檢查您的AdobeMarketo Engage版以瞭解功能可用性。

>[!AVAILABILITY]
>
>用星表示的特徵(![星](assets/yellow-star.png))是付費附加項。 請聯繫您的Marketo Engage代表以瞭解詳細資訊。

**_季度發佈_**

以下功能將開始在 **2022年3月11日**，在接下來的幾週內（除非另有指定）分階段部署每項功能。

## 跨通道業務流程 {#cross-channel-orchestration}

* **動態聊天**:通過主動、有趣和1:1的個性化對話，將銷售線索和客戶作為目標，最大限度地利用您網站上的所有機會。 [動態聊天](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target=&quot;_blank&quot;}允許Marketo Engage用戶開始利用聊天作為B2B市場營銷和銷售使用案例的跨渠道整合體驗的關鍵部分。 功能包括：直接在聊天中預訂會議、引導路由、入門模板、拖放對話建立等。 動態聊天包含在所有Marketo Engage包中，並將於今年向所有Marketo Engage用戶推出。

* **電子郵件Bot活動篩選增強**:作為對先前發佈的 [電子郵件Bot活動篩選](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target=&quot;_blank&quot;}功能，您現在可以選擇登錄已標識為bot的日誌記錄活動。 然後，您可以根據已標識為由bot執行的活動來篩選和觸發操作。

## 新一代體驗 {#next-generation-experience}

* **新一代體驗中的更新螢幕**:我們將提供新一代體驗中的更多刷新螢幕，提供可通過切換開關進行的更新設計和可用性增強：

   * Design Studio中的「電子郵件清單」視圖（包括新的批量操作）
   * Design Studio中的「表單清單」視圖（包括新的批量操作）

* **導入程式工作流更新**:導入程式工作流正在以新一代體驗提供，同時還更新了設計和可用性增強功能。 這將是自動更改，不使用切換開關。

* **新一代體驗切換交換機的管理控制**:管理新一代體驗的推廣，以便管理員能夠選擇哪些用戶類型可以訪問切換開關的用戶。

## 體驗自動化 {#experience-automation}

* **自助服務流步驟(Beta)**:通過編寫自定義流步驟以便在智慧市場活動中使用，擴展Marketo Engage與堆棧其餘部分之間的連接。 Marketo用戶和合作夥伴都可以利用此功能，允許在批處理和可執行活動中使用外部Web服務，而Webhook只能用於觸發活動。

* **資產到期**:保持對時間敏感型資產和市場活動的控制，並能夠在「傳統」用戶體驗中的指定日期和時間安排其自動停用。

* **智慧市場活動優先順序覆蓋**:確保高優先順序觸發的智慧市場活動能夠覆蓋標準市場活動優先順序等級，從而盡快執行。 低優先順序觸發的智慧市場活動也可以降低優先順序，以釋放處理資源用於其他高優先順序任務。

## API增強 {#api-enhancements}

* **返回禁用開啟的電子郵件跟蹤狀態**:允許通過API讀取電子郵件的開啟跟蹤狀態
* **從電子郵件中檢索動態內容主題行**:使營銷人員能夠在BI工具中執行動態主題行分析
* **程式成員自定義欄位CRUD**:允許商家以寫程式方式建立程式成員自定義欄位
* **批量自定義對象導出已更新的At篩選器**:允許商家以寫程式方式同步自定義對象
* **公開電子郵件程式的開頭設定**:允許營銷人員通過API配置具有提前啟動功能的電子郵件程式
* **選擇性程式標籤更新**:使營銷人員能夠推送選擇性標籤更新，而無需同時推送所有標籤
* **批量活動提取操作結果欄位**:允許營銷人員標識跳過或失敗的活動

**_在整個季度發佈_**

以下功能處於非季度週期，將在未來幾個月中發佈。

## 比齊布爾 {#bizible}

![（星號）](assets/yellow-star.png)

* **BI模板**:Bizible現在將為Tableau和Power BI提供可下載、基本的報告工件和示例報告，以便能夠快速開發定制報告，這些報告適合您的特定業務需求。

## 銷售連接 {#sales-connect}

![（星號）](assets/yellow-star.png)

* **電子郵件連接限制(GA)**:電子郵件連接限制允許銷售連接管理員在將Gmail或Exchange用作您的傳遞渠道時配置電子郵件的發送速率，以便將電子郵件移交給傳遞渠道提供商的速率不超過強制限制。

## 公告 {#announcements}

* **Marketo Sky棄用**:在3月，Marketo Sky將不再可用，因為我們將資源集中在提供下一代用戶體驗上。 為了保持對目前Marketo Sky所獨有的功能的訪問權限，我們將「資產到期」和「智慧市場活動優先順序改寫」引入「經典」體驗。 [按一下這裡](https://nation.marketo.com/t5/the-next-generation-experience/marketo-sky-deprecation-notice/ba-p/320115#M33) 來瞭解更多資訊。

**_產品發佈網路研討會_**

2022年5月11日，上午9:00 PT /下午12:00 PM, [即時網路研討會](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html) 由我們的產品團隊主持，您可以在此學習如何使用所有最新的產品創新。
