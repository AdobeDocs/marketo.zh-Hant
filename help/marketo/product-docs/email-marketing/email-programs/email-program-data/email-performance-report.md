---
unique-page-id: 2359467
description: 電子郵件效能報表 — Marketo檔案 — 產品檔案
title: 以電子郵件傳送效能報表
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 1%

---

# 以電子郵件傳送效能報表 {#email-performance-report}

若要檢視您的電子郵件含統計資料（如已傳遞、已開啟、已點按等）的執行狀況，請建立電子郵件效能報表。

1. [在方案中建立報告](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md)並選取&#x200B;**[!UICONTROL Email Performance]** [報告型別](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md)。
1. [變更報表時間範圍](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md)，然後按一下&#x200B;**[!UICONTROL Report]**&#x200B;標籤。
1. 您到了！ 現在瀏覽報告，檢視電子郵件的執行方式。

   >[!NOTE]
   >
   >「寄件日期」篩選條件是以電子郵件第一個寄件日期為基礎。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >按一下電子郵件的名稱，以在電子郵件預覽器中開啟它。

   >[!NOTE]
   >
   >電子郵件效能報表包含適用於所有人員的活動，包括自電子郵件傳送後已刪除的活動。 有時候，您只想檢視活躍人士的活動。 在這種情況下，您需要從報表中篩選刪除的人員。 使用&#x200B;**[!UICONTROL Smart List]**&#x200B;索引標籤為報告[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)。 如果您未篩選任何特定欄位，請將電子郵件地址篩選器設為： **[!UICONTROL is not empty]**。

   [選取報表欄](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md)以取得電子郵件效能報表包含：

   <table><thead>
<tr>
    <th>欄</th>
    <th>說明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>硬退回</td>
    <td>電子郵件因永久狀況而遭拒，例如電子郵件地址不存在。</td>
  </tr>
  <tr>
    <td>軟退信</td>
    <td>電子郵件因暫時狀況而遭到拒絕，例如伺服器關機或收件匣已滿。</td>
  </tr>
  <tr>
    <td>待處理</td>
    <td>此數字的計算方式為從傳送的總數中減去已傳送、已退信和已軟退信的電子郵件數。</td>
  </tr>
  <tr>
    <td>已點按連結</td>
    <td>按一下電子郵件中連結的電子郵件收件者人數。</td>
  </tr>
  <tr>
    <td>退訂</td>
    <td>按一下電子郵件中「取消訂閱」連結並填寫表單的電子郵件收件者人數。</td>
  </tr>
  <tr>
    <td>已中止</td>
    <td>無法傳送且未收到退回事件的電子郵件數量。 如果在傳送電子郵件後的三天內未收到回應，則電子郵件會自動稱為已中止。</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>在電子郵件中點按的取消訂閱連結和電子郵件地址，將不會在報告中的「已點按連結」下註冊。

一般而言，我們會嘗試用常識來記錄這些統計資料。 例如，如果有人按一下電子郵件中的連結，很明顯他們會先開啟電子郵件。 我們遵循電子郵件效能報表的下列特定規則：

* **規則1**：每個電子郵件活動記錄都設為下列其中一項，且僅設為一項： _已傳遞_、_已硬退回_、_已軟退回_&#x200B;或&#x200B;_擱置中_。

* **規則2**：如果電子郵件記錄顯示&#x200B;*[!UICONTROL Opened]*，則計為&#x200B;*已傳遞*。

* **規則3**：如果電子郵件記錄顯示&#x200B;_[!UICONTROL Clicked Email]_&#x200B;或_[!UICONTROL Unsubscribed]_，則計為&#x200B;_已傳遞_&#x200B;及&#x200B;_已開啟_。

* **規則4**：如果電子郵件為&#x200B;_[!UICONTROL Opened]_，則會忽略退信。 如果電子郵件尚未開啟，_&#x200B;硬退信&#x200B;_優先於_&#x200B;軟退信&#x200B;_和_&#x200B;已傳遞&#x200B;_。

* **規則5**：如果在電子郵件活動傳送三天後未收到任何電子郵件活動，則視為&#x200B;_已中止_。

>[!NOTE]
>
>* 從相同行銷活動傳送給相同人員的多個傳送只會計算一次。
>
>* 來自不同行銷活動的多個傳送至相同人員會個別計算。

>[!MORELIKETHIS]
>
>* [在行銷活動電子郵件報告中篩選Assets](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [篩選電子郵件效能報告中已刪除/合併的記錄](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [電子郵件連結效能報告](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
