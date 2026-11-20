---
description: 瞭解個人層級的電子郵件追蹤覆寫如何讓您控制每個人的電子郵件開啟和點選追蹤，以支援同意和隱私權要求。
title: 個人層級的電子郵件追蹤
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/kF-5V-G6-xr3uV-NQBTmFNfhQnk-r-RYt-v0HvJ-4Go'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a913c84b1c4f8927c951af685884edfc792ff213
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 2%
---
# 個人層級的電子郵件追蹤 {#email-tracking-at-person-level}

人員層級的電子郵件追蹤覆寫可讓您在Marketo環境層級套用預設，然後變更個別人員的預設。 開啟追蹤和點選追蹤是獨立控制。

當您的隱私權要求或組織政策需要同意才能追蹤電子郵件參與時，請使用此功能。

>[!IMPORTANT]
>
>此功能提供的控制可協助支援您的合規義務；它不會決定適用哪些法律或哪些人需要提供同意。 與您的法律和隱私權團隊合作，決定如何設定追蹤，以及如何收集及保留同意。

## 追蹤決策的運作方式 {#how-tracking-decisions-work}

三種設定可搭配使用：

| 設定 | 平準 | 它有什麼作用？ |
|---|---|---|
| **個人層級的電子郵件追蹤覆寫** | 環境 | 開啟或關閉功能。 關閉時，Marketo Engage會忽略環境預設和人員覆寫欄位，並使用正常的追蹤行為。 |
| **電子郵件追蹤預設為關閉** | 環境 | 設定開啟和點選追蹤的預設值。 停用時，預設為開啟追蹤。 啟用時，追蹤預設為關閉。 |
| **覆寫開啟追蹤預設值**&#x200B;和&#x200B;**覆寫點選追蹤預設值** | 人員 | 布林值人員欄位。 `true`的值與該追蹤型別的環境預設值相反。 `false`的值或空值會遵循環境預設值。 |

覆寫欄位本身並不表示「選擇加入」或「選擇退出」。 **`true`一律表示「環境預設值相反」。**

### 追蹤決策表 {#tracking-decision-table}

Marketo Engage會將此決定個別套用至電子郵件開啟和電子郵件點按。

| 功能 | 環境預設值 | 人員覆寫為`false`或空白 | 人員覆寫為`true` |
|---|---|---|---|
| 開啟 | 預設為追蹤 | 已追蹤 | 未追蹤 |
| 開啟 | 預設為追蹤 | 未追蹤 | 已追蹤 |
| 關閉 | 不適用 | 一般追蹤；忽略覆寫和預設 | 一般追蹤；忽略覆寫和預設 |

### 範例 {#example}

假設功能已開啟，且環境預設為追蹤開啟。 人員的&#x200B;**覆寫開啟追蹤預設值**&#x200B;設定為`true`，而&#x200B;**覆寫點選追蹤預設值**&#x200B;是空的。 Marketo Engage不會追蹤該人員的電子郵件開啟次數，但會繼續追蹤其電子郵件點按次數。

## 選擇追蹤模型 {#choose-a-tracking-model}

在啟用功能或填入人員欄位之前，選擇符合您的同意和隱私權要求的模式。

| 模型 | 環境預設值 | 設定覆寫為`true`，當 | 一般使用 |
|---|---|---|---|
| 選擇退出 | 預設為追蹤 | 要追蹤的人員物件 | 追蹤大部分的人，但停止追蹤提出物件的人。 |
| 選擇加入（同意） | 預設為追蹤 | 同意追蹤的人 | 追蹤前必須先取得同意，包括適用的CNIL或Garante指引所涵蓋的收件者。 |

>[!CAUTION]
>
>在填入覆寫欄位之前選擇您的模型，並避免在之後變更環境預設值。 因為`true`表示「與預設值相反」，變更預設值會反轉每個現有覆寫值的效果。 例如，從預設開啟追蹤切換到預設關閉追蹤，可能會使之前反對追蹤的人受到追蹤。 如果您必須變更預設值，請在變更生效之前更新所有受影響人員的覆寫值。

## 啟用功能 {#enable-the-feature}

個人層級的電子郵件追蹤覆寫預設為關閉。 若要啟用此功能，請聯絡Adobe客戶支援。 您也可以指定Marketo環境的功能預設狀態是&#x200B;**已啟用**&#x200B;或&#x200B;**已停用**。

>[!NOTE]
>
>您必須是Marketo管理員才能提交此請求。

>[!TIP]
>
>在要求Adobe啟用此功能之前，請填入現有人員的覆寫欄位。 這可協助確保在啟用後準備的第一封電子郵件會套用預期的追蹤行為。

## 設定人員的覆寫值 {#set-override-values-for-people}

覆寫欄位是布林值人員欄位。 使用適合您工作流程的方法設定它們：

| 方法 | 附註 |
|---|---|
| [變更資料值流程步驟](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value){target="_blank"} | 當個人符合您的條件時（例如提交表單上的同意核取方塊），使用Smart Campaign設定欄位。 |
| 表單 | 將Marketo Engage表單上的核取方塊或隱藏欄位對應到人員欄位。 |
| 清單匯入 | 在匯入檔案中將欄位加入為欄。 |
| REST API | 使用API欄位名稱`overrideOpenTrackingDefault`和`overrideClickTrackingDefault`。 |

根據個人的同意設定每個欄位。 如果您的同意語言會個別處理開啟和點按，請個別設定每個欄位。

## 電子郵件中的變更 {#what-changes-in-the-email}

當Marketo Engage不追蹤個人時，它會變更傳送給該人的電子郵件內容。

| 已關閉的追蹤 | 哪些變更 | 仍然有效的功能 |
|---|---|---|
| 開啟次數 | 電子郵件不包含開啟追蹤畫素。 未記錄任何&#x200B;**開啟電子郵件**&#x200B;活動。 | 其他電子郵件功能，包括點選追蹤（如果保持啟用）。 |
| 點按次數 | 連結會直接前往其目的地，而非透過Marketo Engage追蹤網域。 隱藏的追蹤連結未新增。 沒有記錄任何&#x200B;**點選電子郵件**&#x200B;活動。 | 取消訂閱連結、電子郵件頁尾選擇退出連結、`list-unsubscribe`以及&#x200B;**以網頁檢視**&#x200B;連結繼續運作。 使用這些連結不會錄製&#x200B;**按一下電子郵件**&#x200B;活動。 |

## 哪些電子郵件會受到影響 {#which-emails-are-affected}

| 電子郵件類型 | 是否套用覆寫？ |
|---|---|
| 批次電子郵件，例如從批次Smart Campaign或電子郵件程式傳送的電子郵件 | 是 |
| 觸發電子郵件，例如從觸發程式Smart Campaign傳送的電子郵件 | 是 |
| 包含A/B測試或冠軍/挑戰者變體的電子郵件 | 是的。 系統會分別決定每個人的追蹤，無論他們收到哪種變體。 |
| 以網頁檢視 | 是的。 網頁版本會遵循使用者目前的設定。 變更最多需要一小時的時間才會顯示。 |
| [營運電子郵件](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational){target="_blank"} | 否。 他們遵循一般的追蹤行為。 |
| 範例（測試）電子郵件 | 否。 他們遵循一般的追蹤行為。 |
| 電子郵件預覽 | 無變更。 不會追蹤預覽。 |
| 警示電子郵件 | 無變更。 不會追蹤警報。 |
| SMS訊息 | 否。 此功能僅適用於電子郵件。 |

## Marketo Engage進行追蹤決策時 {#when-marketo-engage-makes-the-tracking-decision}

Marketo Engage在準備要傳送的電子郵件時讀取人員的覆寫值。

- **已排程或延遲的傳遞：**&#x200B;如果電子郵件現在已準備且稍後傳遞（例如，具有[開始時間](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs){target="_blank"}或[收件者時區](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone){target="_blank"}），則適用準備時的值。 準備後進行的變更不會變更該電子郵件。
- **已傳遞的電子郵件：**&#x200B;變更人員的覆寫並不會變更他們已收到的電子郵件。 如果先前傳送的電子郵件中的連結已準備並啟用追蹤，仍可追蹤這些連結的點按次數。
- **未來的電子郵件：**&#x200B;變更套用至Marketo Engage在變更後準備的電子郵件。

如果人員撤回同意，請儘快更新其覆寫值，以便將變更套用至為他們準備的下一封電子郵件。

## 對報表、智慧列示和評分的影響 {#impact-on-reporting-smart-lists-and-scoring}

當Marketo Engage未追蹤人員時，它不會記錄&#x200B;**開啟電子郵件**&#x200B;或&#x200B;**按一下電子郵件**&#x200B;活動。 因此：

- **智慧清單/行銷活動：**&#x200B;篩選器和觸發器（例如&#x200B;**已開啟電子郵件**&#x200B;和電子郵件中的&#x200B;**點按連結**）不符合或觸發（如果未追蹤對應的活動）。
- **報表和控制面板：**&#x200B;電子郵件開啟率、點按率和連結效能只會反映追蹤的人員。 參與量度可能會因為有更多人未受到追蹤而減少。
- **評分和方案成功：**&#x200B;根據開啟或點按的規則和方案成功步驟不適用於未追蹤活動的人員。 檢閱這些規則，以免他人受到不公平的評分或進階。
- **網頁活動關聯：**&#x200B;點選追蹤關閉時，電子郵件連結不會附帶Marketo Engage追蹤權杖。 如果Munchkin尚未知道此人，則不會透過連結將此電子郵件的網站造訪與此人建立關聯。

>[!NOTE]
>
>已傳送、已傳遞、已退回和已取消訂閱的活動不受影響。

## 如何與其他追蹤設定搭配使用 {#how-this-works-with-other-tracking-settings}

個人層級的電子郵件追蹤覆寫可以關閉個人的追蹤。 當其他設定已停用追蹤時，它不會開啟追蹤。 例如，即使此人的設定允許點選追蹤，標示為`mktNoTrack`類別的連結仍會維持未追蹤狀態。

## 停用功能 {#disable-the-feature}

若要停用個人層級的電子郵件追蹤覆寫，請聯絡Adobe客戶支援。

>[!NOTE]
>
>您必須是Marketo管理員才能提交此請求。

停用後，在變更後準備的電子郵件會恢復正常追蹤行為。 覆寫值會保留在人員記錄上，但會被忽略。 如果稍後再次啟用該功能，則儲存的值會再次套用。

## 常見問題 {#frequently-asked-questions}

### 我可以追蹤開啟次數但不追蹤個人的點按次數嗎？反之亦然？ {#can-i-track-opens-but-not-clicks-for-a-person-or-the-reverse}

是的。 開啟和點選追蹤是獨立決定的。 僅設定您要變更之追蹤型別的覆寫欄位。

### 此功能是否阻止我傳送電子郵件給某人？ {#does-this-feature-stop-me-from-sending-emails-to-a-person}

否。 它只會控制追蹤。 若要停止傳送行銷電子郵件給個人，請使用現有的取消訂閱和同意功能。

### 未追蹤的人員仍會看到正在處理的取消訂閱連結嗎？ {#do-people-who-are-not-tracked-still-see-working-unsubscribe-links}

是的。 取消訂閱連結和&#x200B;**以網頁檢視**&#x200B;連結仍適用於所有人員。

### 為什麼選擇退出的人員仍然有點選電子郵件活動？ {#why-does-a-person-who-opted-out-still-have-a-click-email-activity}

訪客很可能按一下電子郵件中的連結，而該電子郵件是在其覆寫值變更前就已準備好。 變更套用至變更後準備的電子郵件。

### 是否需要變更我的電子郵件範本？ {#do-i-need-to-change-my-email-templates}

否。 Marketo Engage在建置每封電子郵件時會套用追蹤決定。 您不需要變更範本或電子郵件。
