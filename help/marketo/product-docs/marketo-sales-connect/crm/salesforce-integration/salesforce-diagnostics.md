---
unique-page-id: 14745730
description: Salesforce診斷——行銷檔案——產品檔案
title: Salesforce診斷
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---


# Salesforce診斷 {#salesforce-diagnostics}

我們的Salesforce整合包括Web應用程式中的Salesforce診斷頁面。 此頁面會從失敗的Salesforce資料記錄中擷取錯誤。 這些錯誤可能有用，但並不總是可讀的。 因此，我們會整理出有助於解釋錯誤訊息的速查表。

**錯誤：** API_CURRENTLY_DISABLED\
**類別：** 存取／驗證\
**訊息：** 此使用者的API已停用\
**發生了什麼：** 使用者沒有API存取權\
**疑難排解步驟：** Salesforce管理員需要授與使用者API存取權。

<br> 

**錯誤：** 驗證失敗\
**類別：** 驗證\
**訊息：** invalid_grant:驗證失敗\
**發生了什麼：** 驗證失敗\
**疑難排解步驟：** 與Salesforce斷開連線，然後重新連線。

<br> 

**錯誤：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**類別：** 存取／驗證\
**訊息：** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Session expired or invalid&quot;}\
**發生了什麼：**

1 —— 觸發程式碼導致更新失敗。\
2 —— 用戶對給定對象沒有對象級寫入權限。

**疑難排解步驟：**

1 —— 查看失敗的觸發器。\
2 —— 將對象的寫訪問權限授予用戶，或禁用嘗試寫入對象的功能。

<br> 

**錯誤：** CANNOT_UPDATE_CONVERTED_LEAD\
**類別：** 其他\
**訊息：** 無法參考轉換的銷售線索\
**發生了什麼：** 我們嘗試在聯繫人和銷售線索的最近活動記錄期間登錄到已轉換的銷售線索。 還看過幾個推銷的例子。\
**疑難排解步驟：** 請向我們的支援團隊報告任何 [情況](http://nation.marketo.com/community/support_solutions)。

<br> 

**錯誤：** ENTITY_IS_LOCKED\
**類別：** 存取／驗證\
**訊息：** 圖元已鎖定以供編輯\
**發生了什麼：** 該記錄正處於核准程式中，在核准程式中，記錄會被鎖定，直到擁有核准之人核准或拒絕為止。\
**疑難排解步驟：** 請參閱上文。

<br> 

**錯誤：** EXPIRED_ACCESS類&#x200B;**別：** 驗證&#x200B;**消息：** invalid_grant:過期存取／重新整理Token **發生的情況：** 存取或重新整理Token已過期。 預付碼會根據Salesforce [中的作業設定到期](http://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via)。
**疑難排解步驟：** 您需要重新驗證。 斷開Salesforce連線並重新連線。

<br> 

**錯誤：** FAILED_WRITE\
**類別：** 間歇性\
**訊息：** 到達檔案結尾\
**發生了什麼：** Salesforce的效能問題，可能是由於客戶端的次最佳觸發因素所致。\
**疑難排解步驟：** 重試邏輯應處理此問題。 如果仍無法運作，請與您的Salesforce管理員合作，疑難排解有問題的觸發器。

<br> 

**錯誤：** FIELD_CUSTOM_VALIDATION_EXCEPTION類&#x200B;**別：** 存取／驗證&#x200B;**訊息：** 因客戶而異。
**發生了什麼：** 失敗物件的自訂驗證規則。
**疑難排解步驟：** 檢查導致此錯誤的自訂驗證規則。 由於這是自訂規則，因此必須一次性處理錯誤。

<br> 

**錯誤：** FIELD_FILTER_VALIDATION_EXCEPTION\
**類別：** 存取／驗證\
**訊息：** 值不存在或不符合篩選條件\
**發生了什麼：** 更新時，Salesforce中現有的不良資料會被強制執行。\
**疑難排解步驟：** 請參閱上文。

<br> 

**錯誤：** FIELD_INTEGRITY_EXCEPTION\
**類別：** 存取／驗證\
**訊息：** 現有國家／地區不識別欄位的州值：州／省代碼\
**發生了什麼：** 更新時，Salesforce中現有的不良資料會被強制執行。\
**疑難排解步驟：** 請參閱上文。

<br> 

**錯誤：** 非活動組織\
**類別：** 驗證\
**訊息：** invalid_grant:非活動組織\
**發生了什麼：** 您的Salesforce組織不再有效。\
**疑難排解步驟：** 斷開連接，然後重新連接到Salesforce。

**錯誤：** INACTIVE_USER類&#x200B;**別：** 驗證&#x200B;**消息：** invalid_grant:非活動用&#x200B;**戶發生的情況：** Salesforce使用者不再使用疑難排解&#x200B;**步驟：** 斷開連接，然後重新連接到Salesforce。

**錯誤：** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**類別：** 間歇性\
**訊息：** （無其他訊息）\
**發生了什麼：** Salesforce例項處於維護模式。\
**疑難排解步驟：** 等待系統維護完成，然後重試記錄。

**錯誤：** INDEFIC_ACCESS_ON_CROSS_REFERENCE_ENTITY **類別：** 存取／驗證&#x200B;**訊息：** 物件ID的存取權限不足&#x200B;**發生的情況：** 無法訪問任務的父記錄。
**疑難排解步驟：** 請參閱上文。

<br> 

**錯誤：** INDEFIC_ACCESS_OR_READONLY\
**類別：** 存取／驗證** **訊&#x200B;**息：** 物件ID的存取權限不足** ****發生的情況：** 「最近的活動記錄」無法編輯特定記錄，因為使用者沒有寫入存取權。\
**疑難排解步驟：** 授與使用者在Salesforce中的存取權，或停用該使用者對象的最新活動記錄。

**錯誤：** 無效欄位\
**類別：** 間歇性\
**訊息：** 網：:ReadTimeout\
**發生了什麼：** 請求逾時。 這可能是交易太慢的結果。\
**疑難排解步驟：** 審查潛在潛在的潛在罪魁禍首的現有定制設定，並／或禁用一個或多個對象的「最近活動」日誌，以減少負載。

**錯誤：** INVALID_FIELD_FOR_INSERT_UPDATE\
**類別：** 存取／驗證\
**訊息：** 無法建立／更新欄位：ToutApp_Tout_Last_Resloded__c。請檢查此欄位的安全設定。\
**發生了什麼：** 使用者沒有執行「最近活動」記錄交易所需之「輸出」自訂欄位的寫入存取權。 團隊可能已安裝軟體包，但未為用戶啟用正確的欄位。\
**疑難排解步驟：** Salesforce管理員需要授與自訂欄位的存取權，或關閉「最近活動記錄」。

**錯誤：** INVALID_GRANT\
**類別：** 驗證\
**訊息：** invalid_grant:受限制\
**發生了什麼：** 我們嘗試存取您的Salesforce，但您有IP限制，使我們無法存取。\
**疑難排解步驟：** 您的Salesforce管理員需要允許列出我們的IP。 使用者應聯絡「支援」以取得IP位址。

**錯誤：** 無效類型\
**類別：** 存取／驗證\
**訊息：** CreatedDate,（從任務中選擇ID）FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Column:53s不支援物件類型&#39;Lead&#39;。 如果您嘗試使用自訂物件，請務必在實體名稱后附加「__c」。 請參考您的WSDL或說明呼叫，以取得適當的名稱\
**發生了什麼：** 我們嘗試從Salesforce查詢使用者無權存取的物件類型。 這很可能與使用者沒有權限存取銷售機會物件有關。\
**疑難排解步驟：** 在Salesforce中授與Lead物件的「讀取」和「更新」存取權，或關閉電子郵件記錄和「最近活動記錄」以記錄銷售機會。

**錯誤：** QUERY_TIMEOUT\
**類別：** 間歇性\
**訊息：** 您的查詢請求執行時間過長\
**發生了什麼：** 請參閱上文。\
**疑難排解步驟：** 重試邏輯應處理此問題。 如果仍無法運作，請與您的Salesforce管理員合作，疑難排解有問題的觸發器。

**錯誤：** REQUEST_LIMIT_EXCEEDED\
**類別：** 間歇性\
**訊息：** 1 —— 超出ConcurrentPerOrgLongTxn限制\
2 —— 超出總請求數限制\
3 - ConcurrentRequest\
**發生了什麼：** 1 —— 超出並行請求限制，可能是因為觸發程式碼效率不彰。\
2 —— 太多整合讓組織超過24小時滾動視窗。\
**疑難排解步驟：** 1 —— 查看受影響對象的現有觸發器。 可能會停用一或多個物件的統計記錄。\
2 —— 向Salesforce購買更多API呼叫。 可能會停用一或多個物件的統計記錄。

**錯誤：** REQUIRED_FIELD_MISSING\
**類別：** 存取／驗證\
**訊息：** 必填欄位遺失： [Amount_Committed_Private_Capital_c]\
**發生了什麼：** 這通常發生在「最近活動記錄」中。 自訂欄位已設定為必填，但其中有空值。 如果建立的記錄具有自定義欄位的空值，然後是必需的，則可能會發生這種情況。 我們嘗試更新記錄時會強制要求，即使我們未觸及自訂欄位。\
**疑難排解步驟：** 手動更新遺失欄位的值。 然後，您可以重試ToutApp中的訊息。

**錯誤：** SERVER_UNAVAILABLE\
**類別：** 間歇性\
**訊息：** 伺服器太忙\
**發生了什麼：** Salesforce的效能問題，可能是由於客戶的次最佳觸發\
**疑難排解步驟：** 重試邏輯應處理此問題。 如果仍無法運作，請與您的Salesforce管理員合作，以無法拍出有問題的觸發器。

**錯誤：** TXN_SECURITY_NO_ACCESS\
**類別：** 存取／驗證\
**訊息：** 由於貴組織有安全性原則，因此您請求的作業不允許。 聯絡您的管理員。\
**發生了什麼：** 已設定某種安全限制——請參閱 `https://developer.salesforce.com/forums/?id="record` ID」\
**疑難排解步驟：** 與您的Salesforce管理員交談，瞭解特定限制。

**錯誤：** UNABLE_TO_LOCK_ROW\
**類別：** 間歇性\
**訊息：** 無法獲得對此記錄或1條記錄的獨佔訪問權：&quot;記錄ID&quot;\
**發生了什麼：** 可能是有觸發器導致多次嘗試存取相同的記錄，可能是群組電子郵件。\
**疑難排解步驟：** 重試邏輯應處理此問題。 如果仍無法運作，請與您的Salesforce管理員合作，疑難排解有問題的觸發器。

**錯誤：** UNKNOWN_EXCEPTION\
**類別：** 其他\
**訊息：** 發生未知異常\
**發生了什麼：** Salesforce中未處理的異常。\
**疑難排解步驟：** 使用Salesforce歸檔案例，並複製錯誤訊息中的數值。 這是Salesforce代碼無法正確處理錯誤。
