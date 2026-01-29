---
unique-page-id: 2359467
description: 電子郵件績效報告 - Marketo 文件 - 產品文件
title: 電子郵件績效報告
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '489'
ht-degree: 100%

---

# 電子郵件績效報告 {#email-performance-report}

若要查看您的電子郵件在傳遞、開啟、點擊等統計資料方面的表現，請建立電子郵件績效報告。

1. [在方案中建立報告](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md)並選取&#x200B;**[!UICONTROL Email Performance]** [報告類型](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md)。
1. [變更報告時間範圍](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md)，然後按一下 **[!UICONTROL Report]** 索引標籤。
1. 您完成了！現在探索報告，查看電子郵件的執行方式。

   >[!NOTE]
   >
   >「寄件日期」篩選器的根據為傳送電子郵件的第一個日期。

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >按一下電子郵件的名稱，即可在電子郵件預覽器中將其開啟。

   >[!NOTE]
   >
   >電子郵件績效報告包含適用於所有人員的活動，包括傳送電子郵件後即已刪除的活動。有時候，您可能只想查看活躍人員的活動。在這種情況下，您需要從報告中篩選已刪除的人員。使用 **[!UICONTROL Smart List]** 索引標籤來為報告[建立智慧清單](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)。如果您並未篩選任何特定欄位，則請將電子郵件地址篩選器設為：**[!UICONTROL is not empty]**。

   電子郵件績效報告的[選取報告欄](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md)，包含：

   <table><thead>

<tr>
    <th>欄</th>
    <th>說明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>已硬退回</td>
    <td>電子郵件因永久性狀況而遭拒絕，例如電子郵件地址不存在。</td>
  </tr>
  <tr>
    <td>已軟退回</td>
    <td>電子郵件因暫時性狀況而遭到拒絕，例如伺服器關機或收件匣已滿。</td>
  </tr>
  <tr>
    <td>待處理</td>
    <td>此數字是以已傳送總數減去已傳遞、已退回及已軟退回的電子郵件數目後計算得出。</td>
  </tr>
  <tr>
    <td>已點按的連結</td>
    <td>已點按電子郵件中連結的電子郵件收件者數目。</td>
  </tr>
  <tr>
    <td>已取消訂閱</td>
    <td>已點按電子郵件中「取消訂閱」連結並填寫表單的電子郵件收件者數目。</td>
  </tr>
  <tr>
    <td>已中止</td>
    <td>無法傳遞且未收到退回事件的電子郵件數目。如果在傳送電子郵件後的三天內未收到回應，則系統會自動將電子郵件標記為「已中止」。</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>在電子郵件中按一下取消訂閱連結和電子郵件地址，這些連結即不會計入報告中的「已點按連結」。

一般而言，我們會設法運用常識來記錄這些統計資料。例如，如果有人點按了電子郵件中的連結，他們顯然已經先開啟了電子郵件。我們會遵循電子郵件績效報告的下列特定規則：

* **規則 1**：每個電子郵件活動記錄只能設定為下列其中一項：_已傳遞_、_已硬退回_、_已軟退回_&#x200B;或&#x200B;_待處理_。

* **規則 2**：如果電子郵件記錄顯示 _[!UICONTROL Opened]_，則計為_&#x200B;已傳遞&#x200B;_。

* **規則 3**：如果電子郵件記錄顯示 _[!UICONTROL Clicked Email]_或_[!UICONTROL Unsubscribed]_，則計為&#x200B;_已傳遞_&#x200B;及&#x200B;_已開啟_。

* **規則 4**：如果電子郵件為 _[!UICONTROL Opened]_，則會忽略退回。如果電子郵件還未開啟，_&#x200B;已硬退回&#x200B;_會優先於_&#x200B;已軟退回&#x200B;_和_&#x200B;已傳遞&#x200B;_。

* **規則 5**：如果傳送電子郵件三天後未收到任何電子郵件活動，則將其視為&#x200B;_已中止_。

>[!NOTE]
>
>* 從相同行銷活動至相同人員的多個傳送只會計算一次。
>
>* 從不同的行銷活動至相同人員的多個傳送則會分別計算。

>[!MORELIKETHIS]
>
>* [篩選行銷活動電子郵件報告中的資產](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [篩選電子郵件績效報告中已刪除/已合併的記錄](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [電子郵件連結效能報告](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
