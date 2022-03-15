---
description: Salesforce診斷 — Marketo文檔 — 產品文檔
title: Salesforce診斷
hide: true
hidefromtoc: true
source-git-commit: 94f89e64b69d3997effe6736241a68f8314db1e6
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Salesforce診斷 {#salesforce-diagnostics}

我們的Salesforce整合的一部分包括Web應用程式中的Salesforce診斷頁。 此頁捕獲到Salesforce的失敗資料記錄中的錯誤。 這些錯誤可能有用，但並不總是可讀。 因此，我們整理了一個幫助解釋錯誤消息的作弊表。

## 訪問診斷 {#access-diagnostics}

1. 按一下齒輪表徵圖，然後選擇 **設定**。

   ![](assets/salesforce-diagnostics-1.png)

1. 在「整合」下，按一下 **診斷**。

   ![](assets/salesforce-diagnostics-2.png)

## 錯誤作弊表 {#error-cheat-sheet}

**錯誤：** API_CURRENT_DISABLED\
**類別：** 訪問/驗證\
**消息：** 此用戶已禁用API\
**正在發生的事情：** 用戶沒有API訪問權限\
**故障排除步驟：** Salesforce Admin需要授予用戶API訪問權限。

**錯誤：** 驗證失敗\
**類別：** 驗證\
**消息：** 無效_grant:驗證失敗\
**正在發生的事情：** 身份驗證失敗\
**故障排除步驟：** 斷開與Salesforce的連接，然後重新連接。

**錯誤：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**類別：** 訪問/驗證\
**消息：** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;會話已過期或無效&quot;}\
**正在發生的事情：**

1 — 觸發器代碼導致更新失敗。\
2 — 用戶對給定對象沒有對象級寫入權限。

**故障排除步驟：**

1 — 查看失敗的觸發器。\
2 — 為對象授予用戶寫權限，或禁用嘗試寫入對象的功能。

**錯誤：** CANNOT_UPDATE_CONVERTED_LEAD\
**類別：** 其他\
**消息：** 無法引用轉換的線索\
**正在發生的事情：** 我們嘗試在聯繫人和線索的最近活動記錄期間登錄到轉換的線索。 還看過幾個這樣的投球。\
**故障排除步驟：** 請向我們報告此情況 [支援團隊](https://nation.marketo.com/t5/Support/ct-p/Support)。

**錯誤：** 實體_IS_LOCKED\
**類別：** 訪問/驗證\
**消息：** 實體被鎖定以進行編輯\
**正在發生的事情：** 該記錄處於審批流程中，在其中，它會從任何其他編輯中被鎖定，直到其被擁有審批的人批准或拒絕。\
**故障排除步驟：** 見上。

**錯誤：** 過期訪問(_A)
**類別：** 驗證
**消息：** 無效_grant:過期訪問/刷新令牌
**正在發生的事情：** 訪問或刷新令牌已過期。 令牌根據 [Salesforce中的會話設定](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via)。
**故障排除步驟：** 你需要重新驗證。 斷開Salesforce連接並重新連接。

**錯誤：** 失敗_寫入\
**類別：** 間歇\
**消息：** 已到達檔案結尾\
**正在發生的事情：** Salesforce的效能問題，可能是由於客戶端的觸發器不夠優化。\
**故障排除步驟：** 重試邏輯應處理此問題。 如果它仍不工作，請與Salesforce管理員一起解決有問題的觸發器。

**錯誤：** FIELD_CUSTOM_VALIDATION_EXCEPTION
**類別：** 訪問/驗證
**消息：** 因客戶而異。
**正在發生的事情：** 未通過對象的自定義驗證規則。
**故障排除步驟：** 檢查導致此錯誤的自定義驗證規則。 由於這是自定義規則，因此必須一次性處理錯誤。

**錯誤：** FIELD_FILTER_VALIDATION_EXCEPTION\
**類別：** 訪問/驗證\
**消息：** 值不存在或與篩選條件不匹配\
**正在發生的事情：** 更新時Salesforce中現有的錯誤資料將被強制執行。\
**故障排除步驟：** 見上。

**錯誤：** FIELD_INTEGRITY_EXCEPTION\
**類別：** 訪問/驗證\
**消息：** 現有國家/地區不承認欄位的狀態值：州/省代碼\
**正在發生的事情：** 更新時Salesforce中現有的錯誤資料將被強制執行。\
**故障排除步驟：** 見上。

**錯誤：** 非活動組織\
**類別：** 驗證\
**消息：** 無效_grant:無效組織\
**正在發生的事情：** 您的Salesforce組織不再處於活動狀態。
**故障排除步驟：** 斷開連接，然後重新連接Salesforce。

**錯誤：** 非活動用戶
**類別：** 驗證
**消息：** 無效_grant:非活動用戶
**正在發生的事情：** Salesforce用戶不再處於活動狀態
**故障排除步驟：** 斷開連接，然後重新連接Salesforce。

**錯誤：** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**類別：** 間歇\
**消息：** （沒有其他消息）\
**正在發生的事情：** Salesforce實例處於維護模式。\
**故障排除步驟：** 等待系統維護完成，然後重試記錄。

**錯誤：** 不足_ACCESS_ON_CROSS_REFERENCE_ENTITY
**類別：** 訪問/驗證
**消息：** 對象ID的訪問權限不足
**正在發生的事情：** 無法訪問任務的父記錄。
**故障排除步驟：** 見上。

**錯誤：** 不足_ACCESS_OR_READONLY\
**類別：** 訪問/驗證
**消息：** 對象ID的訪問權限不足
**正在發生的事情：** 由於用戶沒有寫入訪問權限，最近的活動日誌記錄無法編輯特定記錄。\
**故障排除步驟：** 在Salesforce OR為該用戶的對象禁用最新活動日誌記錄中授予用戶訪問權限。

**錯誤：** 無效欄位\
**類別：** 間歇\
**消息：** 網路：:ReadTimeout\
**正在發生的事情：** 請求正在超時。 這可能是交易太慢的結果。\
**故障排除步驟：** 查看潛在的潛在潛在事件源的現有自定義設定，並/或禁用一個或多個對象的最新活動日誌記錄以減少負載。

**錯誤：** INVALID_FIELD_FOR_INSERT_UPDATE\
**類別：** 訪問/驗證\
**消息：** 無法建立/更新欄位：MSE_Rexpled__c。請檢查此欄位的安全設定。
**正在發生的事情：** 用戶沒有對執行最近活動日誌記錄事務所需的Sales Insight Actions自定義欄位的寫權限。 團隊可能已安裝包，但尚未為用戶啟用正確的欄位。\
**故障排除步驟：** Salesforce管理員需要授予對自定義欄位的訪問權限或關閉最近活動日誌記錄。

**錯誤：** INVALID_GRANT\
**類別：** 驗證\
**消息：** 無效_grant:IP限制\
**正在發生的事情：** 我們正嘗試訪問您的Salesforce，但您有IP限制，阻止我們訪問。\
**故障排除步驟：** 您的Salesforce管理員需要允許列出我們的IP。 用戶應聯繫「支援」以獲得IP地址。

**錯誤：** 無效類型\
**類別：** 訪問/驗證\
**消息：** CreatedDate，（從任務中選擇ID）FROM Lead WHERE電子郵件=&#39;emailid&#39;^ERROR:1:不支援列：53s對象類型「Lead」。 如果嘗試使用自定義對象，請確保在實體名稱后附加「__c」。 請參考您的WSDL或描述調用，以獲取相應的名稱
**正在發生的事情：** 我們試圖從Salesforce查詢用戶無權訪問的對象類型。 這很可能與用戶沒有權限訪問Lead對象有關。\
**故障排除步驟：** 對Salesforce中的Lead對象授予「讀取」和「更新」訪問權限，或關閉電子郵件記錄和「最近活動記錄」以記錄潛在客戶記錄。

**錯誤：** 查詢超時\
**類別：** 間歇\
**消息：** 您的查詢請求運行時間過長\
**正在發生的事情：** 見上。\
**故障排除步驟：** 重試邏輯應處理此問題。 如果它仍不工作，請與Salesforce Admin一起解決有問題的觸發器。

**錯誤：** REQUEST_LIMIT_EXCEEDED\
**類別：** 間歇\
**消息：**
1 — 超過ConcurrentPerOrgLongTxn限制\
2 — 超過TotalRequests限制\
3 — 併發請求\
**正在發生的事情：**
1 — 超過併發請求限制，可能是由於觸發器代碼效率低下。\
2 — 太多的整合使組織超過24小時滾動窗口。\
**故障排除步驟：**
1 — 查看受影響對象的現有觸發器。 可能禁用一個或多個對象的匯總日誌記錄。\
2 — 從Salesforce購買更多API調用。 可能禁用一個或多個對象的匯總日誌記錄。

**錯誤：** REQUIRED_FIELD_MISSING\
**類別：** 訪問/驗證\
**消息：** 缺少必填欄位： `[Amount_Committed_Private_Capital__c]`
**正在發生的事情：** 這通常發生在最近的活動日誌記錄中。 自定義欄位設定為必填，但其中包含空值。 如果建立的記錄具有自定義欄位的空值，並且該記錄是必需的，則可能會發生這種情況。 在嘗試更新記錄時，即使未觸及自定義欄位，也會強制要求。\
**故障排除步驟：** 手動更新缺少欄位的值。 然後，您可以從Sales Insight Actions重試消息。

**錯誤：** 伺服器不可用\
**類別：** 間歇\
**消息：** 伺服器太忙\
**正在發生的事情：** Salesforce的效能問題，可能是由於客戶觸發的次優觸發器\
**故障排除步驟：** 重試邏輯應處理此問題。 如果它仍不能正常工作，請與您的Salesforce Admin合作，以便無法觸發有問題的觸發器。

**錯誤：** TXN_SECURITY_NO_ACCESS\
**類別：** 訪問/驗證\
**消息：** 由於您組織中的安全策略，不允許您請求的操作。 請與管理員聯繫。
**正在發生的事情：** 已設定某種安全限制 — 請參閱https://developer.salesforce.com/forums/?id=「記錄ID」\
**故障排除步驟：** 與您的Salesforce Admin聯繫，瞭解具體限制是什麼。

**錯誤：** UNABLE_TO_LOCK_ROW\
**類別：** 間歇\
**消息：** 無法獲得對此記錄或1條記錄的獨佔訪問權限：&quot;記錄ID&quot;\
**正在發生的事情：** 可能有觸發器導致多次嘗試訪問同一記錄，在組電子郵件中可能是如此。\
**故障排除步驟：** 重試邏輯應處理此問題。 如果它仍不工作，請與Salesforce Admin一起解決有問題的觸發器。

**錯誤：** UNKNOWN_EXCEPTION
**類別：** 其他\
**消息：** 發生未知異常\
**正在發生的事情：** Salesforce中未處理的異常。\
**故障排除步驟：** 使用Salesforce將案例存檔並複製錯誤消息中的數值。 這是Salesforce代碼未正確處理錯誤。
