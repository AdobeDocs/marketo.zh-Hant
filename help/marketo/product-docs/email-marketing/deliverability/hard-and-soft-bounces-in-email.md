---
unique-page-id: 1147328
description: 電子郵件中的硬跳出和軟跳出 — Marketo檔案 — 產品檔案
title: 電子郵件中的硬跳出和軟跳出
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 電子郵件中的硬跳出和軟跳出 {#hard-and-soft-bounces-in-email}

當郵件伺服器通知Marketo無法傳遞某人的電子郵件時，硬跳出可能會導致該人的電子郵件地址無效。 軟跳出表示傳送電子郵件給人員時發生錯誤；此問題會自動解決，有時需要幾天時間。 硬跳出和軟跳出都包含 [多個類別](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## 跳出分類 {#bounce-classification}

Marketo中有5個人員字串與問題電子郵件傳送有關。

1. **電子郵件已暫停**  — 發生特定型別的硬跳出時，設為True。
1. **電子郵件暫停原因**  — 原因有很多。 此欄位會嘗試說明原因。
1. **電子郵件暫停時間：**  — 當發生違反規定的反彈時，Marketo將暫停郵寄給此人員24小時（從此時間戳記）。
1. **電子郵件無效**  — 發生特定型別的硬跳出時，設為True。
1. **電子郵件無效原因**  — 硬跳出的原因。

>[!NOTE]
>
>個人到達後 **電子郵件已暫停** 狀態，無法清除「電子郵件已暫停」核取方塊。 不過，該人士在首次被停職24小時後仍會保持郵寄狀態。
>
>當人員標示為 **電子郵件無效**，則只能透過取消核取其紀錄的「人員資訊」索引標籤中的「電子郵件無效」方塊來手動重設（建議您僅在您知道其電子郵件有效時才會這樣做）。

>[!PREREQUISITES]
>
>追隨 [這些步驟](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) 建立將產生退回資料的電子郵件效能報表。

建立電子郵件效能報表後，您的畫面應該看起來像這樣：

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>垃圾郵件篩選器有時會產生硬退信。 這些「誤判」並不表示該人員電子郵件地址的真實有效性。
