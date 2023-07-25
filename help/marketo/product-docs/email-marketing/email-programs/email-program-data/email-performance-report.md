---
unique-page-id: 2359467
description: 電子郵件效能報表 — Marketo檔案 — 產品檔案
title: 電子郵件效能報表
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# 電子郵件效能報表 {#email-performance-report}

若要檢視您的電子郵件使用已傳送、已開啟、已點按等統計資料的執行狀況，請建立電子郵件效能報表。

1. [在方案中建立報告](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) 並選取 **電子郵件效能** [報表型別](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [變更報表時間範圍](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) 並按一下 **報告** 標籤。
1. 您到了！ 現在瀏覽報告，檢視電子郵件的執行方式。

   >[!NOTE]
   >
   >「傳送日期」篩選條件以電子郵件的第一個傳送日期為基礎。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >按一下電子郵件的名稱，以在電子郵件預覽器中開啟它。

   >[!NOTE]
   >
   >電子郵件效能報表包含適用於所有人員的活動，包括自電子郵件傳送後已刪除的活動。 有時候，您只想檢視活躍人士的活動。 在這種情況下，您需要從報表中篩選刪除的人員。 使用 **智慧清單** 按Tab鍵至 [建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 以取得報表。 如果您未篩選任何特定欄位，請將電子郵件地址篩選器設為： **不是空的**.

   [選取報表欄](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) 電子郵件效能報表包含：

   | 欄 | 說明 |
   |---|---|
   | 硬退回 | 電子郵件因永久條件而遭到拒絕，例如電子郵件地址不存在。 |
   | 軟退信 | 電子郵件因暫時狀況（例如伺服器關閉或收件匣已滿）而遭到拒絕。 |
   | 待處理 | 此數字的計算方式是從已傳送的總數減去已傳送、已退信和已軟退信的電子郵件數。 |
   | 已點按連結 | 按一下電子郵件中連結的電子郵件收件者人數。 |
   | 退訂 | 按一下「 」的電子郵件收件者人數 **取消訂閱** 連結並填寫表單。 |

   >[!NOTE]
   >
   >取消訂閱在電子郵件中被點按的連結和電子郵件地址，將不會在報告中的「已點按連結」下註冊。

一般而言，我們會嘗試用常識來記錄這些統計資料。 例如，如果有人按一下電子郵件中的連結，很明顯他們會先開啟電子郵件。 我們遵循電子郵件效能報表的下列特定規則：

* **規則1**：每個電子郵件活動記錄都會設為下列其中一項（且僅為一項）： _已傳遞_， _硬退回_， _軟退信_，或 _擱置中_.

* **規則2**：如果電子郵件記錄顯示 *已開啟*，即計為 *已傳遞*.

* **規則3**：如果電子郵件記錄顯示 _已點按的電子郵件_ 或 _已取消訂閱_，即計為 _已傳遞_ 和 _已開啟_.

* **規則4**：如果電子郵件為 _已開啟_，會忽略退信。 如果電子郵件尚未開啟， _硬退回_ 優先於 _軟退信_ 和 _已傳遞_.

>[!NOTE]
>
>從相同行銷活動傳送至相同人員的多個傳送只會計算一次。

>[!MORELIKETHIS]
>
>* [在Campaign電子郵件報告中篩選資產](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [以電子郵件傳送連結效能報表](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)
