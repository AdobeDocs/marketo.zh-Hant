---
unique-page-id: 1147328
description: 電子郵件中的硬性和軟性彈回數——行銷檔案——產品檔案
title: 電子郵件中的硬彈回數和軟彈回數
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# 電子郵件中的硬彈回數和軟彈回數 {#hard-and-soft-bounces-in-email}

當郵件伺服器告訴Market無法傳送該人員的電子郵件時，硬彈回數會導致該人員的電子郵件地址無效。 彈跳的柔和意味著，將電子郵件傳送給對方時出了問題；這會自動解決，有時需要數天。 硬性彈回數和軟性彈回數皆由多 [個類別組成](http://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838)。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## 反彈分類 {#bounce-classification}

Marketo中有5個人字串與問題電子郵件傳送有關。

1. **Email Suspended** —— 當發生特定類型的硬彈回時，設為True。
1. **電子郵件暫停原因** -可能有許多原因。 這個欄位會試著解釋原因。
1. **電子郵件暫停於**-發生違規彈回時，Marketo將暫停寄送給該人24小時的郵件時間。
1. **電子郵件無效** -當發生特定類型的硬彈回時，設為True。
1. **電子郵件無效原因** -出現硬彈回的原因。

>[!NOTE]
>
>當某人達到電子郵 **件暫停狀態** 後，便無法清除電子郵件暫停核取方塊。 不過，在最初停職24小時後，此人仍將可以郵寄。
>
>當某人被標示為電子郵件無 **效**，則只能透過取消勾選其記錄「人員資訊」標籤中的「電子郵件無效」方塊，手動重設他們（建議您僅在您知道其電子郵件是否有效時才重設）。

>[!NOTE]
>
>**必要條件**
>
>請依 [照下列步驟](../../../product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) ，建立會產生彈回資料的「電子郵件效能報表」。

建立「電子郵件效能報表」後，您的螢幕應該如下所示： ![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>垃圾訊息篩選器有時會建立硬彈回數。 這些「誤報」並不表示該人的電子郵件地址真實有效。

