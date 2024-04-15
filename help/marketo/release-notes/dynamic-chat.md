---
description: Dynamic Chat發行說明 — Marketo檔案 — 產品檔案
title: Dynamic Chat發行說明
hide: true
hidefromtoc: true
feature: Release Information, Dynamic Chat
source-git-commit: c2c95f36c710ba7a9ac75c2160c72e44b5f81a99
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# 發行說明： 2024年4月 {#release-notes-apr-24}

Adobe Dynamic Chat版本會在持續傳遞模式上運作，允許以更可擴充的方法進行功能部署。 有時候一個月會有多個版本，所以請定期回來檢視最新的資訊。

Marketo Engage的標準發行說明頁面 [可在此處找到](/help/marketo/release-notes/current.md){target="_blank"}.

## 4月發行 {#april-release}

**發行日期： 2024年4月16日**

### Select套件的客戶現在可以使用對話流程 {#conversational-flows-select-package}

去年我們發佈Conversational Flows時，Dynamic ChatSelect套件的客戶只能利用這項功能，進行100個期限參與測試。 現在，Select套件中的所有客戶都可使用對話流程。

對話式流程參與將計入Select套件中客戶每月最多250個參與對話的次數上限中。

### 回呼函式 {#callback-functions}

當訪客參與Dynamic Chat對話時，回呼函式可讓您收集外部系統(例如Adobe Analytics或Google Analytics)中的Dynamic Chat分析事件。 您可以使用API註冊回呼來監聽事件，藉此啟用Dynamic Chat分析事件。 這可讓您以更整體的方式檢視與其他關鍵資料（例如網站流量）相關的Dynamic Chat參與。

### 即時代理程式可用性條件已新增到條件式分支 {#live-agent-availability-conditional-branching}

除了原生和自訂Marketo欄位以外，您現在還可以使用條件式分支，根據代理程式可用性建立分支。 如果您只想讓訪客在有可用的即時代理程式時選擇與即時代理程式交談，這個功能會很有用。

熒幕擷圖

### 智慧清單條件已新增到條件式分支 {#smart-list-condition}

在條件式分支中新增新的「Marketo Engage智慧列示」條件後，您就可以根據已在Marketo中建立的現有對象建立分支，而非在Dynamic Chat中定義對象分支條件。

熒幕擷圖

### 對話流程的條件式分支 {#conditional-branching-for-conversational-flows}

我們今年早些時候發佈了對話的條件分支，現在您也可以利用對話流程中的條件分支！ 條件式分支可讓您根據不同的條件在流程中建立分支。

### 對話流程的即時聊天 {#live-chat-for-conversational-flows}

我們去年發佈了對話的即時聊天功能，現在您也可以將即時聊天參與新增到對話流程中。 如果您搭配Marketo表單使用對話流程，您現在可以允許合格訪客在表單提交後立即與即時代理程式聊天！

### 代理程式收件匣中最近的Marketo Engage活動 {#recent-marketo-engage-activities-in-agent-inbox}

我們已將最近的Marketo Engage活動新增到「代理程式收件匣」的「最近的活動」區段，這樣當網站訪客請求與代理程式聊天時，代理程式就能輕鬆檢視訪客最近是否參與了下列任何Marketo活動（過去25個活動）：

* 已開啟的電子郵件
* 造訪的網頁
* 已填寫的表單
* 曾有過關鍵時刻

熒幕擷圖

### 代理程式管理中的行事曆連線狀態 {#calendar-connection-status-in-agent-management}

管理員現在可以輕鬆檢視哪些具有會議預訂許可權的代理已以Dynamic Chat連線其行事曆。 這可讓您確保您的整個銷售團隊都已連線，且準備好接受Dynamic Chat的會議邀請。

熒幕擷圖

### 代理程式行事曆設定中的最低通知設定 {#minimum-notice-setting-in-agent-calendar-configuration}

客戶回報網站訪客在其行事曆上預約會議，只會收到10分鐘的預先通知，因此我們在代理程式行事曆設定中引進了最低通知設定，並將預設前置時間設為24小時。

熒幕擷圖

### 新應用程式內通知 {#new-in-app-notifications}

我們已推出三種新的應用程式內通知，協助您即時瞭解Dynamic Chat例項的狀態。

* 文字
* 文字
* 文字

### 新增/移除使用者行為已更新 {#add-remove-user-behavior-updated}

有些客戶向我們告知在Dynamic Chat中新增和移除代理程式時遇到的問題，因此我們進行了一些變更以解決這些問題。

當使用者新增到具有即時聊天或會議預約許可權的Admin Console時，他們將立即出現在「代理管理」清單中，並可用於新增到對話方塊、對話流程、路由規則和團隊。

當具有會議預約或即時聊天許可權的使用者從Admin Console中移除時，他們將會立即從Dynamic Chat中移除，將無法再用於即時聊天或會議路由，並且不再計入授許可權制。

### 改善交談層級報告效能 {#improved-conversation-level-report-performance}

「個別對話方塊」和「對話流量」層級報表現在可提供更有效且更準確的資料。 以前，對話方塊報表可能需要幾秒鐘的時間才能載入，而且資料有時與全域效能報表不一致。 現在，您的個別對話方塊報表將會立即載入，而且資料將一律與全域報表資料對齊。

熒幕擷圖

### 許可權更新 {#permission-updates}

我們已清除Adobe Admin Console中的許可權結構和命名，讓許可權管理更直覺化。

* 「交談管理」類別現在稱為「交談」
* 會議類別現在稱為活動
* 代理程式設定類別現在稱為代理程式
* 「管理員設定」類別現在稱為「設定」
* 即時聊天類別已移除，且所有即時聊天許可權已移至代理程式類別

熒幕擷圖

### 支援代理程式收件匣中的超連結 {#support-for-hyperlinks-in-agent-inbox}

現在，當即時聊天代理程式與聊天中的訪客共用URL時，這些URL將會超連結，以便訪客只需按一下這些URL即可導覽至頁面，而不必將URL複製並貼到瀏覽器中。

### 在代理程式收件匣中輸入更新的金鑰行為 {#enter-key-behavior-updated-in-agent-inbox}

我們已切換「代理程式收件匣」中的傳回鍵行為，因此按Return或Enter鍵會傳送您的訊息，而按Shift+Enter鍵則會建立分行符號。

熒幕擷圖

### 循環配置資源頁面已移除 {#round-robin-page-removed}

別擔心！ 循環配置資源路由仍然完全正常運作，而且運作方式與以往一樣。 我們剛剛移除了在循環配置資源路由佇列中顯示經常不正確代理程式清單及其順序的頁面。

為了提供一些情境，當我們在2022年發佈Dynamic Chat時，沒有提供即時聊天支援，只有會議預約和循環配置資源路由頁面在設計時考慮到了會議預約。 隨著去年即時聊天功能的推出，循環配置資源頁面已過時，因為它無法準確反映同時具有會議預約和即時聊天許可權之代理程式之間循環配置資源路由的更複雜性質。 我們探索了一些不同的選項來解決此問題，但最終決定完全移除它是最小化混淆的最佳選項。

## 2月發行 {#february-release}

**發行日期： 2024年2月22日**

### 對話頁面 {#conversations-page}

新的「交談」頁面為您提供了一站式服務，讓您檢視執行個體發生的所有交談（自動化和即時）記錄（來自已知和匿名潛在客戶），讓您更清楚地瞭解客戶如何與您的對話、交談流程和即時代理進行互動。

熒幕擷圖

全域控制面板中的日期範圍從90天增加到24個月

您詢問，我們已送達。 您現在可以在所有Analytics儀表板中檢視長達兩年的Dynamic Chat參與資料。

### 對話方塊中的條件分支 {#conditional-branching-in-dialogues}

條件式分支可讓您根據不同的條件，在對話方塊流程中建立分支。 現在，您可以根據Marketo中的銷售機會和公司屬性，在相同對話方塊中向不同人員呈現不同的內容。

## 1月發行 {#january-release}

**發行日期： 2024年1月24日**

### 代理程式管理中的同時即時聊天限制設定 {#Concurrent-live-chat-limit-setting}

依預設，您執行個體中的每個即時聊天代理程式一次最多可以參與5個即時聊天工作階段。 我們在代理程式管理中引進了新的設定，可讓您調整此限制，從1到10不等。

熒幕擷圖
