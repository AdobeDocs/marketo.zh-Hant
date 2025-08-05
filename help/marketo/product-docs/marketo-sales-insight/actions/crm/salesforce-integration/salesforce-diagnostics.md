---
description: Salesforce診斷 — Marketo檔案 — 產品檔案
title: Salesforce診斷
exl-id: c449f938-9615-47cb-b232-613ec29068a3
feature: Sales Insight Actions
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '1339'
ht-degree: 0%

---

# [!DNL Salesforce]診斷 {#salesforce-diagnostics}

我們[!DNL Salesforce]整合的一部分包含網頁應用程式中的[!DNL Salesforce]診斷頁面。 此頁面會擷取記錄到[!DNL Salesforce]的失敗資料中的錯誤。 錯誤可能會有所幫助，但並不一定可讀取。 因此，我們會收集速查表來協助說明錯誤訊息。

## 存取診斷 {#access-diagnostics}

1. 按一下齒輪圖示並選擇&#x200B;**[!UICONTROL Settings]**。

   ![](assets/salesforce-diagnostics-1.png)

1. 在[!UICONTROL Integrations]底下，按一下&#x200B;**[!UICONTROL Diagnostics]**。

   ![](assets/salesforce-diagnostics-2.png)

## 錯誤速查表 {#error-cheat-sheet}

**錯誤：** API_CURRENTLY_DISABLED
**類別：**存取/驗證
**訊息：** API已針對此使用者停用
**發生狀況：**使用者沒有API存取權
**疑難排解步驟：** [!DNL Salesforce]管理員需要授與使用者API存取權。

**錯誤：**驗證失敗
**類別：**驗證
**訊息：** invalid_grant：驗證失敗
**發生狀況：**驗證失敗
**疑難排解步驟：**&#x200B;中斷與[!DNL Salesforce]的連線，然後重新連線。

**錯誤：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY
**類別：**存取/驗證
**訊息：** {&quot;errorCode&quot;：&quot;INVALID_SESSION_ID&quot;，&quot;message&quot;：&quot;工作階段已過期或無效&quot;}
**正在發生的事情：**

1 — 觸發程式碼導致更新失敗。
2 — 使用者沒有特定物件的物件層級寫入許可權。

**疑難排解步驟：**

1 — 檢閱失敗的觸發器。
2 — 將物件的寫入許可權授與使用者，或是停用嘗試寫入物件的功能。

**錯誤：** CANNOT_UPDATE_CONVERSION_LEAD
**類別：**其他
**訊息：**無法參考轉換的潛在客戶
**發生什麼事：**我們嘗試在連絡人和潛在客戶的最新活動記錄期間，記錄到已轉換的潛在客戶。 也看過這些推介詞。
**疑難排解步驟：**&#x200B;請將此專案的任何執行個體回報給我們的[支援團隊](https://nation.marketo.com/t5/Support/ct-p/Support)。

**錯誤：** ENTITY_IS_LOCKED
**類別：**存取/驗證
**訊息：**實體已鎖定以進行編輯
**發生狀況：**記錄正在核准程式中，除非擁有核准的人員核准或拒絕記錄，否則不會進行任何額外的編輯。
**疑難排解步驟：**&#x200B;請參閱上文。

**錯誤：** EXPIRED_Access
**類別：**驗證
**訊息：** invalid_grant：存取權/重新整理權杖已過期
**發生狀況：**&#x200B;存取或重新整理Token已過期。 Token會根據[ [!DNL Salesforce]中的](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via)工作階段設定到期。
**疑難排解步驟：**&#x200B;您需要重新驗證。 中斷[!DNL Salesforce]連線並重新連線。

**錯誤：** FAILED_WRITE
**類別：**間歇性
**訊息：**已到達檔案結尾
**發生狀況：**&#x200B;發生[!DNL Salesforce]效能問題，可能是因為客戶端的觸發程式未達最佳狀態。
**疑難排解步驟：**&#x200B;重試邏輯應該處理這個問題。 如果仍然無法運作，請和您的[!DNL Salesforce]管理員合作，疑難排解有問題的觸發器。

**錯誤：** FIELD_CUSTOM_VALIDATION_EXCEPTION
**類別：**存取/驗證
**訊息：**因客戶而異。
**發生狀況：**物件的自訂驗證規則失敗。
**疑難排解步驟：**&#x200B;檢查造成此錯誤的自訂驗證規則。 由於這是自訂規則，因此必須一次性處理錯誤。

**錯誤：** FIELD_FILTER_VALIDATION_EXCEPTION
**類別：**存取/驗證
**訊息：**值不存在或不符合篩選條件
**發生狀況：** [!DNL Salesforce]中現有的錯誤資料在更新時強制執行。
**疑難排解步驟：**&#x200B;請參閱上文。

**錯誤：** FIELD_INTEGRITY_EXCEPTION
**類別：**存取/驗證
**訊息：**現有的國家/地區無法辨識欄位的州值：州/省代碼
**發生狀況：** [!DNL Salesforce]中現有的錯誤資料在更新時強制執行。
**疑難排解步驟：**&#x200B;請參閱上文。

**錯誤：** INACTIVE_ORGANIZATION
**類別：**驗證
**訊息：** invalid_grant：非使用中組織
**正在發生的事情：**&#x200B;您的[!DNL Salesforce]組織已不在作用中。
**疑難排解步驟：**&#x200B;中斷連線，然後從[!DNL Salesforce]重新連線。

**錯誤：**非使用中使用者
**類別：**驗證
**訊息：** invalid_grant：非使用中的使用者
**正在發生的事情：** [!DNL Salesforce]使用者已不在作用中
**疑難排解步驟：**&#x200B;中斷連線，然後從[!DNL Salesforce]重新連線。

**錯誤：** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE
**類別：**間歇性
**訊息：** （沒有其他訊息）
**發生狀況：** [!DNL Salesforce]執行個體處於維護模式。
**疑難排解步驟：**&#x200B;等到系統維護完成後再重試記錄。

**錯誤：** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**類別：**存取/驗證
**訊息：**物件識別碼的存取許可權不足
**正在發生的事情：**無法存取任務的父記錄。
**疑難排解步驟：**&#x200B;請參閱上文。

**錯誤：** INSUFFICIENT_ACCESS_OR_READONLY
**類別：**存取/驗證
**訊息：**物件識別碼的存取許可權不足
**發生狀況：**最近活動記錄無法編輯特定記錄，因為使用者沒有寫入許可權。
**疑難排解步驟：**&#x200B;在[!DNL Salesforce]中授與使用者存取權，或停用該使用者最近活動的記錄。

**錯誤：**無效的_FIELD
**類別：**間歇性
**訊息：**網路：：ReadTimeout
**發生狀況：**要求逾時。 這可能是由於太多緩慢交易所致。
**疑難排解步驟：**&#x200B;檢閱現有的自訂，找出延遲問題的可能原因，並/或停用一或所有物件的「最近活動」記錄，以減少負載。

**錯誤：** INVALID_FIELD_FOR_INSERT_UPDATE
**類別：**存取/驗證
**訊息：**無法建立/更新欄位： MSE_Replied__c。請檢查此欄位的安全性設定。
**發生狀況：**使用者沒有執行最近活動記錄交易所需的銷售Insight動作自訂欄位的寫入許可權。 Team可能已經安裝封裝，但尚未為使用者啟用正確的欄位。
**疑難排解步驟：** [!DNL Salesforce]管理員需要授與自訂欄位的存取權，或關閉最近的活動記錄。

**錯誤：** INVALID_GRANT
**類別：**驗證
**訊息：** invalid_grant： ip已限制
**發生狀況：**&#x200B;我們正在嘗試存取您的[!DNL Salesforce]，但您已經設有IP限制，因此無法存取。
**疑難排解步驟：**&#x200B;您的[!DNL Salesforce]管理員必須將IP加入允許清單。 使用者應該聯絡支援以取得IP位址。

**錯誤：** INVALID_TYPE
**類別：**存取/驗證
**訊息：** CreatedDate， （從工作選取ID） FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at `Row:1:Column:53sObject`不支援&#39;Lead&#39;型別。 如果您嘗試使用自訂物件，請務必在實體名稱后附加「__c」。 請參考您的WSDL或描述呼叫以取得適當的名稱
**發生狀況：**我們嘗試從Salesforce查詢使用者無權存取的物件型別。 這很可能是因為使用者沒有正確存取該Lead物件的許可權。
**疑難排解步驟：**&#x200B;授予Salesforce中Lead物件的讀取和更新存取權，或關閉電子郵件記錄和Lead記錄的最近活動記錄。

**錯誤：** QUERY_TIMEOUT
**類別：**間歇性
**訊息：**您的查詢要求執行時間太長
**正在發生的事情：**請參閱上文。
**疑難排解步驟：**&#x200B;重試邏輯應該處理這個問題。 如果仍然無法運作，請與您的[!DNL Salesforce]管理員合作，疑難排解有問題的觸發器。

**錯誤：** REQUEST_LIMIT_EXCEEDED
**類別：**間歇性
**訊息：**
1 — 超過ConcurrentPerOrgLongTxn限制
2 — 超過TotalRequests限制
3 — 並行請求
**正在發生的事情：**
1 — 超過並行請求限制，可能是因為觸發程式碼效率低。
2 — 太多整合將組織置於24小時滾動視窗之外。
**疑難排解步驟：**
1 — 檢閱受影響物件上的現有觸發器。 可能會停用一或多個物件的彙總記錄。
2 — 從[!DNL Salesforce]購買更多API呼叫。 可能會停用一或多個物件的彙總記錄。

**錯誤：** REQUIRED_FIELD_MISSING
**類別：**存取/驗證
**訊息：**&#x200B;缺少必要欄位： `[Amount_Committed_Private_Capital__c]`
**發生的情況：**這通常發生在最近的活動記錄中。 自訂欄位已設定為必填，但內含空白值。 如果記錄是使用自訂欄位的空值建立的，然後設定為必填，則可能會發生這種情況。 當我們嘗試更新記錄時，即使我們未觸及自訂欄位，需求會強制執行。
**疑難排解步驟：**&#x200B;手動更新遺漏欄位的值。 接著，您可以從「銷售Insight動作」重試訊息。

**錯誤：** SERVER_UNAVAILABLE
**類別：**間歇性
**訊息：**伺服器太忙碌
**發生狀況：**&#x200B;發生[!DNL Salesforce]效能問題，可能是因為客戶的觸發程式未達最佳狀態
**疑難排解步驟：**&#x200B;重試邏輯應該處理這個問題。 如果仍然無法運作，請與您的[!DNL Salesforce]管理員合作，疑難排解有問題的觸發器。

**錯誤：** TXN_SECURITY_NO_ACCESS
**類別：**存取/驗證
**訊息：**由於貴組織有安全性原則，因此不允許您要求的作業。 請連絡您的管理員。
**發生狀況：**&#x200B;已設定某種安全性限制 — 請參閱<https://developer.salesforce.com/forums/?id="record>識別碼」
**疑難排解步驟：**&#x200B;請洽詢您的[!DNL Salesforce]管理員，並檢視可能的特定限制。

**錯誤：** UNABLE_TO_LOCK_ROW
**類別：**間歇性
**訊息：**無法取得此記錄的獨佔存取權或1筆記錄：「記錄識別碼」
**發生狀況：**可能是觸發程式導致多次嘗試存取相同的記錄，可能是群組電子郵件。
**疑難排解步驟：**&#x200B;重試邏輯應該處理這個問題。 如果仍然無法運作，請與您的[!DNL Salesforce]管理員合作，疑難排解有問題的觸發器。

**錯誤：** UNKNOWN_EXCEPTION
**類別：**其他
**訊息：**發生未知的例外狀況
**正在發生的情況：**&#x200B;中有[!DNL Salesforce]個未處理的例外狀況。
**疑難排解步驟：**&#x200B;將案例存檔為[!DNL Salesforce]，並複製錯誤訊息中的數值。 這是[!DNL Salesforce]程式碼未正確處理錯誤。
