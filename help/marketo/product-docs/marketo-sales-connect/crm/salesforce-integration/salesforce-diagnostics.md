---
unique-page-id: 14745730
description: Salesforce診斷——行銷檔案——產品檔案
title: Salesforce診斷
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---


# Salesforce診斷{#salesforce-diagnostics}

我們的Salesforce整合包括Web應用程式中的Salesforce診斷頁面。 此頁面會從失敗的Salesforce資料記錄中擷取錯誤。 這些錯誤可能有用，但並不總是可讀的。 因此，我們會整理出有助於解釋錯誤訊息的速查表。

**錯誤：** API_CURRENTLY_DISABLED\
**類別：存** 取／驗證\
**訊息：** 此使用者的API已停用\
**發生什麼：** 使用者沒有API存取權\
**疑難排解步** 驟：Salesforce管理員需要授與使用者API存取權。

<br> 

**錯誤：** AUTHENTICATION_FAILURE\
**類別：驗** 證\
**消息：** invalid_grant:驗證失敗\
**發生什麼：驗** 證失敗\
**疑難排解步** 驟：中斷與Salesforce的連線，然後重新連線。

<br> 

**錯誤：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**類別：存** 取／驗證\
**訊息：** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Session expired or invalid&quot;}\
**發生了什麼：**

1 —— 觸發程式碼導致更新失敗。\
2 —— 用戶對給定對象沒有對象級寫入權限。

**疑難排解步驟：**

1 —— 查看失敗的觸發器。\
2 —— 將對象的寫訪問權限授予用戶，或禁用嘗試寫入對象的功能。

<br> 

**錯誤：** CANNOT_UPDATE_CONVERTED_LEAD\
**類別：其** 他\
**消息：無** 法引用已轉換的銷售線索\
**發生的情況：** 我們嘗試在最近的聯繫人和銷售線索活動記錄期間登錄已轉換的銷售線索。還看過幾個推銷的例子。\
**疑難排解步** 驟：請向我們的支援團隊報告此 [類情況](https://nation.marketo.com/t5/Support/ct-p/Support)。

<br> 

**錯誤：** ENTITY_IS_LOCKED\
**類別：存** 取／驗證\
**消息：** 實體被鎖定以進行編輯\
**正在發生的事** 件：記錄正處於核准程式中，在核准程式中，記錄會被鎖定，直到其被擁有核准的人核准或拒絕為止。\
**疑難排解步驟：** 請參閱上文。

<br> 

**錯誤：** EXPIRED_ACCESS類
**別：驗** 證
**消息：** invalid_grant:過期的存取／重新整
**理Token發生什麼：存** 取或重新整理Token已過期。預付碼會根據Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via)中的[作業設定過期。
**疑難排解** 步驟：您需要重新驗證。斷開Salesforce連線並重新連線。

<br> 

**錯誤：** FAILED_WRITE\
**類別：間歇** 性\
**訊息：** 檔案結束\
**發生什麼：** Salesforce的效能問題，可能是由於客戶端的次最佳觸發因素所致。\
**疑難排解步驟：** 重試邏輯應處理此問題。如果仍無法運作，請與您的Salesforce管理員合作，疑難排解有問題的觸發器。

<br> 

**錯誤：** FIELD_CUSTOM_VALIDATION_EXCEPTION類
**別：訪問／驗證** 消息：
**** 因客戶而異。**發生的情況：** 對象的自訂驗證規則失敗。**疑難排解步** 驟：檢查造成此錯誤的自訂驗證規則。由於這是自訂規則，因此必須一次性處理錯誤。

<br> 

**錯誤：** FIELD_FILTER_VALIDATION_EXCEPTION\
**類別：存** 取／驗證\
**訊息：** 值不存在或不符合篩選條件\
**發生的情況：** Salesforce中現有的不良資料在更新時會被強制執行。\
**疑難排解步驟：** 請參閱上文。

<br> 

**錯誤：** FIELD_INTEGRITY_EXCEPTION\
**類別：存** 取／驗證\
**訊息：** 現有國家／地區不識別欄位的狀態值：州／省代碼\
**發生的情況：** Salesforce中現有的不良資料在更新時會被強制執行。\
**疑難排解步驟：** 請參閱上文。

<br> 

**錯誤：** INACTIVE_ORGANIZATION\
**類別：驗** 證\
**消息：** invalid_grant:非活動組織\
**現狀：您的** Salesforce組織不再有效。\
**疑難排解步** 驟：中斷連線，然後重新連線至Salesforce。

**錯誤：** INACTIVE_USER類
**別：驗** 證
**消息：** invalid_grant:非作用
**中使用者：** Salesforce使用者不再為作用中的疑難排
**解步驟：中斷連線，然** 後重新連線至Salesforce。

**錯誤：** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**類別：間歇** 性\
**訊息：** （無其他訊息）\
**發生什麼：** Salesforce例項處於維護模式。\
**疑難排解步** 驟：等待系統維護完成後再重試記錄。

**錯誤：** INDEFIC_ACCESS_ON_CROSS_REFERENCE_ENTITY類別：訪問／驗證
**消息：對象ID的訪問權限不足** ：發生的情況：
**** 
**** 無權訪問任務的父記錄。**疑難排解步驟：** 請參閱上文。

<br> 

**錯誤：** INDEFIC_ACCESS_OR_READONLY\
**類別：** 存取／驗
**證訊息：** 物件ID的存取權限不足
**** 發生什麼：最新活動記錄無法編輯特定記錄，因為使用者沒有寫入存取權。\
**疑難排解步** 驟：授與使用者在Salesforce中的存取權，或停用該使用者對象的最近活動記錄。

**錯誤：** INVALID_FIELD\
**類別：間歇** 性\
**消息：** Net::ReadTimeout\
**發生什麼：請** 求是逾時。這可能是交易太慢的結果。\
**疑難排解步** 驟：檢查潛在延遲問題的罪魁禍首的現有自訂項目，並／或停用一或所有物件的「最新活動記錄」，以減輕負載。

**錯誤：** INVALID_FIELD_FOR_INSERT_UPDATE\
**類別：存** 取／驗證\
**消息：** 無法建立／更新欄位：ToutApp_Tout_Last_Resloded__c。請檢查此欄位的安全設定。**發生的情況：** 使用者沒有執行「最近活動」記錄交易所需之「輸出」自訂欄位的寫入存取權。團隊可能已安裝軟體包，但未為用戶啟用正確的欄位。\
**疑難排解步** 驟：Salesforce管理員需要授與自訂欄位的存取權，或關閉最近活動記錄。

**錯誤：** INVALID_GRANT\
**類別：驗** 證\
**消息：** invalid_grant:受限制\
**發生什麼：我** 們正嘗試存取您的Salesforce，但您有IP限制，使我們無法存取。\
**疑難排解步** 驟：您的Salesforce管理員需要允許列出我們的IP。使用者應聯絡「支援」以取得IP位址。

**錯誤：** INVALID_TYPE\
**類別：存** 取／驗證\
**消息：** CreatedDate,（從任務中選擇ID）FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Column:53s不支援對象類型&#39;Lead&#39;。如果您嘗試使用自訂物件，請務必在實體名稱后附加「__c」。 請參考您的WSDL或說明呼叫，以取得適當的名稱
**發生的情況：**&#x200B;我們嘗試從使用者無權存取的Salesforce查詢物件類型。 這很可能與使用者沒有權限存取銷售機會物件有關。\
**疑難排解步** 驟：授與Salesforce中Lead物件的讀取和更新存取權，或關閉電子郵件記錄和最近活動記錄以記錄銷售機會。

**錯誤：** QUERY_TIMEOUT\
**類別：間歇** 性\
**訊息：** 您的查詢請求執行時間過長\
**發生了什麼：請** 參閱上面。\
**疑難排解步驟：** 重試邏輯應處理此問題。如果仍無法運作，請與您的Salesforce管理員合作，疑難排解有問題的觸發器。

**錯誤：** REQUEST_LIMIT_EXCEEDED\
**類別：間歇** 性\
**消息：**
1 —— 超出ConcurrentPerOrgLongTxn限制\
2 —— 超出總請求數限制\
3 - ConcurrentRequest\
**發生的情況：**
1 —— 超出並行請求限制，可能是因為觸發程式碼效率不彰。\
2 —— 太多整合讓組織超過24小時滾動視窗。\
**疑難排解步**
驟：1 —— 檢視受影響物件上的現有觸發器。可能會停用一或多個物件的統計記錄。\
2 —— 向Salesforce購買更多API呼叫。 可能會停用一或多個物件的統計記錄。

**錯誤：** REQUIRED_FIELD_MISSING\
**類別：存** 取／驗證\
**訊息：** 必填欄位遺失： `[Amount_Committed_Private_Capital__c]`
**發生的情況：這** 通常發生在最近的活動記錄中。自訂欄位已設定為必填，但其中有空值。 如果建立的記錄具有自定義欄位的空值，然後是必需的，則可能會發生這種情況。 我們嘗試更新記錄時會強制要求，即使我們未觸及自訂欄位。\
**疑難排解步** 驟：手動更新遺失欄位的值。然後，您可以重試ToutApp中的訊息。

**錯誤：** SERVER_UNAVAILABLE\
**類別：間歇** 性\
**消息：服** 務器太忙\
**發生什麼：** Salesforce的效能問題，可能是由於客戶的次最佳觸發\
**疑難排解步驟：** 重試邏輯應處理此問題。如果仍無法運作，請與您的Salesforce管理員合作，以無法拍出有問題的觸發器。

**錯誤：** TXN_SECURITY_NO_ACCESS\
**類別：存** 取／驗證\
**訊息：** 由於貴組織的安全性原則，您請求的作業無法進行。聯絡您的管理員。<br/>
**發生什麼：已** 經設定了某種安全性限制——請參閱https://developer.salesforce.com/forums/?id=「記錄ID」\
**疑難排解步** 驟：與您的Salesforce管理員交談，並瞭解特定限制。

**錯誤：** UNABLE_TO_LOCK_ROW\
**類別：間歇** 性\
**消息：無** 法獲得對此記錄或1條記錄的獨佔訪問權：&quot;記錄ID&quot;\
**發生的事** 件：可能有觸發器導致多次嘗試存取相同記錄，可能是群組電子郵件。\
**疑難排解步驟：** 重試邏輯應處理此問題。如果仍無法運作，請與您的Salesforce管理員合作，疑難排解有問題的觸發器。

**錯誤：** UNKNOWN_EXCEPTION類
**別：其** 他\
**消息：發** 生未知異常\
**發生什麼： Salesforce中** 未處理的異常。\
**疑難排解步** 驟：使用Salesforce將案例歸檔，並複製錯誤訊息中的數值。這是Salesforce代碼無法正確處理錯誤。
