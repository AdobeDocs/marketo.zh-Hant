---
description: 最新發行說明 — Marketo檔案 — 產品檔案
title: 最新發行說明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 4794c44db57b41f6d9358f7e6cc24a41dda68550
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# 發行說明：2022年10月 {#release-notes-oct-22}

以下是』22年10月版本包含的所有功能。 查看您的Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星號表示的特徵(![星星](assets/yellow-star.png))是付費附加元件。 請連絡您的Marketo Engage代表以了解更多資訊。

下列功能將於 **2022年10月14日**，並在後續數週分階段推出剩餘功能（除非另有指定）。 發行功能和確切日期可能會有所變更。

## 跨管道協調 {#cross-channel-orchestration}

* **動態聊天的自動排列對話框流**:透過「自動排列」按鈕，將畫布上的所有內容整理為乾淨且易於閱讀的格式，以改善您擁擠的對話方塊畫布。

* **支援動態聊天的其他資料類型**:三種新的資料類型（布林值、整數、浮點數）可讓您在動態聊天中運用更多現有的Marketo Engage欄位，以執行例如根據分數進行定位或詢問訪客是/否問題。

* **動態聊天的會議連結**:在傳送給訪客的每個日曆邀請中，自動加入Google和Outlook的團隊或集合連結的選項。

* **動態聊天的排程會議通知**:銷售代表會收到有關已排程會議的自動電子郵件通知，以及訪客聊天機器人互動的任何相關資訊。

* **動態聊天的角色和權限**:管理員可以使用精細的權限來控制應用程式的可見性和使用情形，並建立自訂使用者角色。

   * 完全存取 — 使用者可充分運用功能（例如發佈對話方塊、變更色彩配置等）
   * 唯讀存取 — 使用者可以看見資訊但無法變更（例如，請參閱對象條件或資料流設計工具，但不可變更）
   * 限制存取 — 使用者看不到或存取「設定」或「整合」區段

## 新一代體驗 {#next-generation-experience}

* **新一代體驗中的更新畫面**:我們在新一代體驗中提供更多經過更新的畫面，提供可透過切換開關存取的更新設計和可用性增強功能：

   * 登錄頁面範本詳細資訊
   * 電子郵件範本清單

* **增強「電子郵件範本詳細資訊」中的「使用者」索引標籤**:在新體驗中，您會看到使用電子郵件範本之資產的其他相關資訊，包括資產狀態、上次修改時間和上次修改時間。 您也可以搜尋、排序及篩選資產使用的清單。

* **報表資產篩選模組**:新的報表設定模型設計，可在設定功能表中顯示新資產樹，以及「建立日期」和「修改日期」的篩選器。

## 行銷資料環境 {#marketing-data-environment}

* **AdobePrivacy Service整合**:與Privacy Service協調，以自動遵循Experience Cloud產品中的資料隱私權法規。 目前，此服務僅適用於已上線至的Marketo Engage客戶 [AdobeIdentity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target=&quot;_blank&quot;}系統。

* **程式成員自定義欄位同步**:能夠雙向同步為程式成員捕獲的可擴展欄位(例如，在事件註冊期間（如食物、會話、軌道等）的參與者偏好

## API增強功能 {#api-enhancements}

* **批量導入：銷售人員協會**:與Lead REST API平價，以便在大量銷售機會匯入程式期間將銷售機會與Salespers建立關聯，降低複雜性和所需的API呼叫數。

## Sales Insight {#sales-insight}

![（星號）](assets/yellow-star.png)

* **[Sales Insight與動態聊天的整合](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target=&quot;_blank&quot;}**:Insights Dashboard現在包含智慧格線中的動態聊天活動，以及每週摘要和詳細資訊卡。

## 公告 {#announcements}

* **Forms 1.0**:Forms 1.0的淘汰將於10月發行完成。 Forms 1.0資產將無法再將資料提交至Marketo Engage，且若嘗試，將會傳回錯誤。

* **無指令碼Forms**:當瀏覽器中停用Javascript時，Forms將無法繼續運作。 表單提交作業需要啟用Javascript。
