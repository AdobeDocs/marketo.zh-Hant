---
description: Salesforce診斷 — Marketo檔案 — 產品檔案
title: Salesforce診斷
hide: true
hidefromtoc: true
exl-id: c449f938-9615-47cb-b232-613ec29068a3
source-git-commit: d960f0ad0d944bd2e74543f3ab15b59a8040b768
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Salesforce診斷 {#salesforce-diagnostics}

我們的Salesforce整合的一部分包括Web應用程式中的Salesforce診斷頁。 此頁將從失敗的資料記錄中捕獲錯誤到Salesforce。 錯誤可能有用，但並非一律可讀。 因此，我們整理了一張幫助解釋錯誤消息的作弊表。

## 訪問診斷 {#access-diagnostics}

1. 按一下齒輪圖示，然後選擇 **設定**.

   ![](assets/salesforce-diagnostics-1.png)

1. 在整合下方，按一下 **診斷**.

   ![](assets/salesforce-diagnostics-2.png)

## 錯誤速查表 {#error-cheat-sheet}

**錯誤：** API_CURRENTLY_DISABLED\
**類別：** 存取/驗證\
**訊息：** 已針對此使用者停用API\
**發生的狀況：** 使用者沒有API存取權\
**疑難排解步驟：** Salesforce管理員需要授與使用者API存取權。

**錯誤：** AUTHENTICATION_FAILURE\
**類別：** 驗證\
**訊息：** invalid_grant:驗證失敗\
**發生的狀況：** 驗證失敗\
**疑難排解步驟：** 斷開與Salesforce的連接，然後重新連接。

**錯誤：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**類別：** 存取/驗證\
**訊息：** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;會話已過期或無效&quot;}\
**發生的狀況：**

1 — 觸發程式碼導致更新失敗。\
2 — 用戶對給定對象沒有對象級寫入權限。

**疑難排解步驟：**

1 — 檢閱失敗的觸發程式。\
2 — 為對象授予用戶寫入訪問權限，或禁用嘗試寫入對象的功能。

**錯誤：** CANNOT_UPDATE_CONVERTED_LEAD\
**類別：** 其他\
**訊息：** 無法參考轉換的銷售機會\
**發生的狀況：** 我們正嘗試在聯繫人和銷售機會的最近活動記錄期間登錄到轉換的銷售機會。 還看到了幾個投球。\
**疑難排解步驟：** 如有此情況，請向我們的 [支援團隊](https://nation.marketo.com/t5/Support/ct-p/Support).

**錯誤：** ENTITY_IS_LOCKED\
**類別：** 存取/驗證\
**訊息：** 實體已鎖定以進行編輯\
**發生的狀況：** 該記錄處於批准過程中，在獲得批准的人批准或拒絕之前，該記錄將從任何其他編輯中鎖定。\
**疑難排解步驟：** 請參閱上文。

**錯誤：** EXPIRED_ACCESS
**類別：** 驗證
**訊息：** invalid_grant:過期的存取/重新整理權杖
**發生的狀況：** 存取或重新整理Token已過期。 代號的過期時間根據 [Salesforce中的工作階段設定](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**疑難排解步驟：** 你需要重新驗證。 斷開Salesforce連接並重新連接。

**錯誤：** 失敗_寫入\
**類別：** 間歇\
**訊息：** 已到達檔案結尾\
**發生的狀況：** Salesforce的效能問題，可能是因為客戶端的觸發器不佳。\
**疑難排解步驟：** 重試邏輯應處理此問題。 如果仍無法運作，請與Salesforce管理員合作，疑難排解有問題的觸發器。

**錯誤：** FIELD_CUSTOM_VALIDATION_EXCEPTION
**類別：** 存取/驗證
**訊息：** 因客戶而異。
**發生的狀況：** 未通過對象的自定義驗證規則。
**疑難排解步驟：** 檢查導致此錯誤的自訂驗證規則。 由於這是自訂規則，因此必須一次性處理錯誤。

**錯誤：** FIELD_FILTER_VALIDATION_EXCEPTION\
**類別：** 存取/驗證\
**訊息：** 值不存在或不符合篩選條件\
**發生的狀況：** 更新後，Salesforce中的現有錯誤資料會強制執行。\
**疑難排解步驟：** 請參閱上文。

**錯誤：** FIELD_INTEGRITY_EXCEPTION\
**類別：** 存取/驗證\
**訊息：** 現有國家/地區不承認欄位的州值：州/省代碼\
**發生的狀況：** 更新後，Salesforce中的現有錯誤資料會強制執行。\
**疑難排解步驟：** 請參閱上文。

**錯誤：** 非活動組織\
**類別：** 驗證\
**訊息：** invalid_grant:非活動組織\
**發生的狀況：** 您的Salesforce組織不再有效。
**疑難排解步驟：** 斷開連接，然後重新連接Salesforce。

**錯誤：** 非活動用戶
**類別：** 驗證
**訊息：** invalid_grant:非作用中使用者
**發生的狀況：** Salesforce用戶不再活動
**疑難排解步驟：** 斷開連接，然後重新連接Salesforce。

**錯誤：** INSERT_UPDATE_MAINTENANCE_NOT_ALLOWED_DURING_MAINTENANCE\
**類別：** 間歇\
**訊息：** （無其他訊息）\
**發生的狀況：** Salesforce實例處於維護模式。\
**疑難排解步驟：** 等待系統維護完成，然後重試記錄。

**錯誤：** INDEQUIL_ACCESS_ON_CROSS_REFERENCE_ENTITY
**類別：** 存取/驗證
**訊息：** 對象id的訪問權限不足
**發生的狀況：** 無權訪問任務的父記錄。
**疑難排解步驟：** 請參閱上文。

**錯誤：** INDEQUALT_ACCESS_OR_READONLY\
**類別：** 存取/驗證
**訊息：** 對象id的訪問權限不足
**發生的狀況：** 「最近的活動」記錄無法編輯特定記錄，因為用戶沒有寫入權限。\
**疑難排解步驟：** 在Salesforce中授予該用戶訪問權限，或為該用戶禁用該對象的「最近活動」日誌記錄。

**錯誤：** 無效欄位\
**類別：** 間歇\
**訊息：** Net::ReadTimeout\
**發生的狀況：** 請求超時。 這很可能是交易太慢的結果。\
**疑難排解步驟：** 查看潛在延遲問題的罪魁禍首的現有自定義項，和/或禁用一個或多個對象的最近活動日誌以減少負載。

**錯誤：** INVALID_FIELD_FOR_INSERT_UPDATE\
**類別：** 存取/驗證\
**訊息：** 無法建立/更新欄位：MSE_Respled__c。請檢查此欄位的安全設定。
**發生的狀況：** 用戶沒有執行「最近」活動記錄事務處理所需的「銷售分析操作」自定義欄位的寫權限。 團隊可能已安裝軟體包，但未為用戶啟用正確欄位。\
**疑難排解步驟：** Salesforce管理員需要授予自訂欄位的存取權，或關閉最近的活動記錄。

**錯誤：** INVALID_GRANT\
**類別：** 驗證\
**訊息：** invalid_grant:ip受限\
**發生的狀況：** 我們正在嘗試訪問您的Salesforce，但您已設定IP限制，阻止我們訪問。\
**疑難排解步驟：** 您的Salesforce管理員需要允許列出我們的IP。 使用者應聯絡支援以取得IP位址。

**錯誤：** INVALID_TYPE\
**類別：** 存取/驗證\
**訊息：** CREATEDDATE，（從任務中選擇ID）從Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Column:53sObject類型&#39;Lead&#39;不受支援。 如果您嘗試使用自訂物件，請務必在實體名稱后面附加「__c」。 請參考您的WSDL或適當名稱的描述調用
**發生的狀況：** 我們正嘗試從Salesforce查詢用戶無權訪問的對象類型。 這很可能與使用者沒有正確的潛在客戶物件存取權限有關。\
**疑難排解步驟：** 在Salesforce中授予對Lead對象的「讀取」和「更新」訪問權限，或關閉電子郵件日誌記錄和「最近的活動」日誌記錄以提前記錄。

**錯誤：** QUERY_TIMEOUT\
**類別：** 間歇\
**訊息：** 您的查詢請求運行時間太長\
**發生的狀況：** 請參閱上文。\
**疑難排解步驟：** 重試邏輯應處理此問題。 如果仍無法運作，請與Salesforce管理員合作，疑難排解有問題的觸發器。

**錯誤：** REQUEST_LIMIT_EXCEEDED\
**類別：** 間歇\
**訊息：**
1 — 超出ConcurrentPerOrgLongTxn限制\
2 — 已超出總請求數限制\
3 - ConcurrentRequest\
**發生的狀況：**
1 — 超出併發請求限制，可能是因為觸發程式碼效率低下。\
2 — 太多整合讓組織超過24小時滾動視窗。\
**疑難排解步驟：**
1 — 檢閱受影響物件的現有觸發器。 可能禁用一個或多個對象的匯總日誌記錄。\
2 — 從Salesforce購買更多API呼叫。 可能禁用一個或多個對象的匯總日誌記錄。

**錯誤：** REQUIRED_FIELD_MISSING\
**類別：** 存取/驗證\
**訊息：** 缺少必填欄位： `[Amount_Committed_Private_Capital__c]`
**發生的狀況：** 這通常會發生在最近的活動記錄中。 自訂欄位設為必要欄位，但其中有空值。 如果以自訂欄位的空白值建立記錄，然後設為必要，就會發生此情況。 我們嘗試更新記錄時，即使未觸及自訂欄位，也會強制執行要求。\
**疑難排解步驟：** 手動更新缺少欄位的值。 然後，您可以從「銷售分析活動」中重試該消息。

**錯誤：** SERVER_UNAVAILABLE\
**類別：** 間歇\
**訊息：** 伺服器太忙\
**發生的狀況：** Salesforce的效能問題，可能是由於客戶觸發的次最佳觸發\
**疑難排解步驟：** 重試邏輯應處理此問題。 如果仍無法運作，請與您的Salesforce管理員合作，疑難排解有問題的觸發因素。

**錯誤：** TXN_SECURITY_NO_ACCESS\
**類別：** 存取/驗證\
**訊息：** 由於貴組織中的安全策略，不允許您請求的操作。 請聯絡您的管理員。
**發生的狀況：** 已設定某種安全限制 — 請參閱https://developer.salesforce.com/forums/?id=&quot;record ID&quot;\
**疑難排解步驟：** 請洽詢您的Salesforce管理員，了解特定限制可能是什麼。

**錯誤：** UNABLE_TO_LOCK_ROW\
**類別：** 間歇\
**訊息：** 無法獲得對此記錄或1條記錄的獨佔訪問：&quot;記錄ID&quot;\
**發生的狀況：** 可能是有觸發器導致多次嘗試存取相同記錄，在群組電子郵件的情況下。\
**疑難排解步驟：** 重試邏輯應處理此問題。 如果仍無法運作，請與Salesforce管理員合作，疑難排解有問題的觸發器。

**錯誤：** UNKNOWN_EXCEPTION
**類別：** 其他\
**訊息：** 發生未知異常\
**發生的狀況：** Salesforce中未處理的異常。\
**疑難排解步驟：** 使用Salesforce將案例歸檔，並複製錯誤消息中的數值。 這是Salesforce代碼無法正確處理錯誤。
