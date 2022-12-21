---
unique-page-id: 1147328
description: 電子郵件中的硬跳出和軟跳出 — Marketo檔案 — 產品檔案
title: 電子郵件中的硬跳出數和軟跳出數
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 電子郵件中的硬跳出數和軟跳出數 {#hard-and-soft-bounces-in-email}

當郵件伺服器通知Marketo無法傳送人員的電子郵件時，硬退信可能會導致人員的電子郵件地址無效。 軟退信意味著將電子郵件傳送給人時出現問題；這會自動解決，有時需要數天時間。 硬彈回數和軟彈回數均包含 [多個類別](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## 退回分類 {#bounce-classification}

Marketo中有5個與問題電子郵件傳送相關的人員字串。

1. **電子郵件已暫停**  — 當發生特定類型的硬退信時，設為True。
1. **電子郵件已暫停原因**  — 原因有很多。 此欄位試圖解釋原因。
1. **暫停時間的電子郵件**  — 發生違規退信時，Marketo會從此時間戳記起24小時暫停寄送給該人員。
1. **電子郵件無效**  — 當發生特定類型的硬退信時，設為True。
1. **電子郵件無效原因**  — 硬反彈的原因。

>[!NOTE]
>
>當人到達 **電子郵件已暫停** 狀態，則無法清除電子郵件已暫停核取方塊。 不過，在最初暫停後24小時，該人仍可郵寄。
>
>當某人標示為 **電子郵件無效**，則只能透過取消勾選其記錄之「人員資訊」索引標籤中的「電子郵件無效」方塊，手動重設（我們建議您僅在您確定其電子郵件有效時才進行重設）。

>[!PREREQUISITES]
>
>追隨 [這些步驟](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) 若要建立「電子郵件效能報表」，此報表會產生彈回資料。

建立電子郵件效能報表後，您的畫面應該如下所示：

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>垃圾郵件篩選器有時會產生硬跳出。 這些「誤判」並不表示該人員電子郵件地址的真實有效性。
