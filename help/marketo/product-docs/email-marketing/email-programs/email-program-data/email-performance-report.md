---
unique-page-id: 2359467
description: 電子郵件績效報告——行銷人員檔案——產品檔案
title: 電子郵件績效報告
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---


# 電子郵件績效報告 {#email-performance-report}

若要查看您的電子郵件在傳送、開啟、點按等統計資料時的效能，請建立「電子郵件效能報表」。

1. [在程式中建立報表](../../../../product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) ，並選取「電子郵 **件效能**[報表類型」](../../../../product-docs/reporting/basic-reporting/report-types/report-type-overview.md)。
1. [變更「報表時間範圍](../../../../product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) 」，然後按一下「報 **表** 」標籤。
1. 你在那！ 現在請瀏覽報表，瞭解您的電子郵件的執行方式。

   >[!NOTE]
   >
   >「傳送日期」篩選條件是根據電子郵件的第一個傳送日期。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >按一下電子郵件名稱，在「電子郵件預覽器」中將其開啟。

   >[!NOTE]
   >
   >
   >電子郵件績效報表包含所有人的活動，包括自電子郵件傳送以來已刪除的活動。 有時，您只想查看活動中人員的活動。 在這種情況下，您需要從報表中篩選已刪除的人。 使用「 **智慧型清單** 」標籤 [建立報表的智慧型清單](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 。 如果您未在任何特定欄位上進行篩選，請將「電子郵件地址」篩選設為： **不是空的**。

   [為「電子郵件效能](../../../../product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) 」報表選擇報表欄包括：

   | 欄 | 說明 |
   |---|---|
   | 硬性反彈 | 由於電子郵件地址不存在等永久條件，電子郵件被拒絕。 |
   | 軟反彈 | 電子郵件因為暫時狀況而遭拒，例如伺服器關閉或收件匣已滿。 |
   | 待定 | 此數字的計算方式是從「已傳送」總數中減去「已傳送」、「已彈回」和「已軟彈回」的電子郵件數。 |
   | 已點按連結 | 按一下電子郵件中連結的電子郵件收件者數。 |
   | 取消訂閱 | 按一下電子郵件中「取消訂 **閱** 」連結並填寫表單的電子郵件收件者數目。 |

   >[!NOTE]
   >
   >取消訂閱連結和電子郵件中被點按的電子郵件地址不會在報表的「點按連結」下註冊。

總的來說，我們試圖用常識記錄這些統計資料。 例如，如果某人點按了電子郵件中的連結，顯然會先開啟電子郵件。 我們遵循「電子郵件績效報告」的下列特定規則：

* **規則1**:每個電子郵件活動記錄都設為下列其中一項，且僅設為一項： *已交付*、 *硬性已反彈*、軟 *性已反彈*&#x200B;或 *待定*。

* **規則2**:如果電子郵件記錄顯 *示「已開啟*」 *，則會計為「已*&#x200B;傳送」。

* **第3條**:如果電子郵件記錄顯 *示「已點按電子郵件* 」或「未訂 *閱」*，則會計為「已 *傳送* 」和「已 **&#x200B;開啟」。

* **規則4**:如果電子郵件已 *開啟*，則會忽略彈回數。 如果電子郵件尚未開啟，則 *Hard Roburced* 優先於 *Soft Roburced* and *Delivered*。

>[!NOTE]
>
>從相同促銷活動傳送至相同人員的多個促銷活動只會計算一次。

>[!MORELIKETHIS]
>
>* [篩選促銷活動電子郵件報表中的資產](../../../../product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [電子郵件連結效能報告](email-link-performance-report.md)

>



>[!NOTE]
>
>**深入探討**
>
>進一步瞭解基 [本報告](http://docs.marketo.com/display/docs/basic+reporting)。

