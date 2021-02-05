---
unique-page-id: 1147328
description: 電子郵件中的硬性和軟性彈回數——行銷檔案——產品檔案
title: 電子郵件中的硬彈回數和軟彈回數
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# 電子郵件中的硬彈回數和軟彈回數{#hard-and-soft-bounces-in-email}

當郵件伺服器告訴Market無法傳送該人員的電子郵件時，硬彈回數會導致該人員的電子郵件地址無效。 彈跳的柔和意味著，將電子郵件傳送給對方時出了問題；這會自動解決，有時需要數天。 硬彈回數和軟彈回數皆由[多個類別](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838)組成。

## 反彈分類{#bounce-classification}

Marketo中有5個人字串與問題電子郵件傳送有關。

1. **電子郵件暫停** -當發生特定類型的硬彈回時，設為True。
1. **電子郵件暫停原因** -可能有許多原因。這個欄位會試著解釋原因。
1. **電子郵件暫停於** -發生違規反彈時，Marketo將暫停寄送給該人的郵件，從此時間戳記開始24小時。
1. **電子郵件無效** -當發生特定類型的硬彈回時，設為True。
1. **電子郵件無效原因** -出現硬彈回的原因。

>[!NOTE]
>
>當某人達到&#x200B;**電子郵件暫停狀態**&#x200B;後，便無法清除電子郵件暫停複選框。 不過，在最初停職24小時後，此人仍將可以郵寄。
>
>當某人被標籤為&#x200B;**email invalid**&#x200B;時，只能通過取消選中其記錄的「人員資訊」頁籤中的「電子郵件無效」框來手動重設（建議您僅在您知道其電子郵件是否有效時才重設）。

>[!PREREQUISITES]
>
>請依照[這些步驟](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md)建立「電子郵件效能報表」，以產生彈回資料。

建立「電子郵件效能報表」後，您的螢幕應該如下所示：

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>垃圾訊息篩選器有時會建立硬彈回數。 這些「誤報」並不表示該人的電子郵件地址真實有效。
