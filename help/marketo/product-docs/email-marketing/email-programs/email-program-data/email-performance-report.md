---
unique-page-id: 2359467
description: 電子郵件效能報表 — Marketo檔案 — 產品檔案
title: 電子郵件效能報表
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# 電子郵件效能報表 {#email-performance-report}

若要查看您的電子郵件透過傳送、開啟、點按等統計資料的執行狀況，請建立「電子郵件效能報表」。

1. [在方案中建立報表](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) ，然後選取 **電子郵件效能** [報表類型](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [變更報表時間範圍](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) 並按一下 **報表** 標籤。
1. 你在那！ 現在，請探索報表，了解您的電子郵件的執行方式。

   >[!NOTE]
   >
   >「傳送日期」篩選條件是根據電子郵件的第一個傳送日期。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >按一下電子郵件的名稱，以在「電子郵件預覽器」中開啟它。

   >[!NOTE]
   >
   >電子郵件效能報表包含所有人員的活動，包括自電子郵件傳送以來已刪除的活動。 有時候，您只想查看作用中人員的活動。 在此情況下，您需要從報表中篩選已刪除的人員。 使用 **智慧清單** 標籤 [建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) ，即可取得Advertising Cloud的說明。 如果您未篩選任何特定欄位，請將「電子郵件地址」篩選設為： **非空白**.

   [選取報表欄](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) 對於「電子郵件效能」報表，包括：

   | 欄 | 說明 |
   |---|---|
   | 硬跳出 | 由於永久條件（例如不存在的電子郵件地址），電子郵件被拒絕。 |
   | 軟跳出 | 由於臨時條件（如伺服器關閉或收件匣完整），電子郵件遭拒。 |
   | 待處理 | 此數字的計算方式為從「已傳送」總數減去「已傳送」、「已退信」和「已軟退信」的電子郵件數量。 |
   | 已點按連結 | 按一下電子郵件中連結的電子郵件收件者數目。 |
   | 退訂 | 已點按 **取消訂閱** 在電子郵件中連結，並填寫表單。 |

   >[!NOTE]
   >
   >在報表的「已點按連結」底下不會註冊取消訂閱連結和電子郵件地址，只要點按電子郵件即可。

一般來說，我們試圖用常識來記錄這些統計資料。 例如，如果有人按一下電子郵件中的連結，顯然是先開啟電子郵件。 我們在「電子郵件效能報表」中遵循下列特定規則：

* **規則1**:每個電子郵件活動記錄都設為下列其中一個，且僅為一個： _傳遞_, _硬跳出_, _軟跳出_，或 _待定_.

* **規則2**:如果電子郵件記錄顯示 *已開啟*，則會計為 *傳遞*.

* **規則3**:如果電子郵件記錄顯示 _已點按電子郵件_ 或 _已取消訂閱_，則會計為 _傳遞_ 和 _已開啟_.

* **規則4**:如果電子郵件為 _已開啟_，則會忽略彈回數。 如果電子郵件尚未開啟， _硬跳出_ 優先於 _軟跳出_ 和 _傳遞_.

>[!NOTE]
>
>從相同促銷活動傳送至相同人員的多個訊息只會計算一次。

>[!MORELIKETHIS]
>
>* [篩選行銷活動電子郵件報表中的資產](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [電子郵件連結效能報表](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

