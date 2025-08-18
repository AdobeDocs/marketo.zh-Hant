---
unique-page-id: 2359418
description: 匯入人員清單 - Marketo 文件 - 產品文件
title: 匯入人員清單
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 292626741d3b2334da104a515c3e968fb340706a
workflow-type: ht
source-wordcount: '543'
ht-degree: 100%

---

# 匯入人員清單 {#import-a-list-of-people}

## 任務：將商展與會者的試算表清單匯入您的資料庫中 {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[完成設定與新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

在此教學課程中，您會了解如何將試算表檔案中的人員匯入 Marketo 中。

## 步驟 1：下載及編輯試算表 {#step-download-and-edit-a-spreadsheet}

1. 開始時，請將我們的練習用試算表檔案 ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) 下載至您的電腦。

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >匯入日期時，請使用以下格式：**9/21/20** (月/日/年)。

   >[!NOTE]
   >
   >所匯入的任何日期/時間欄位均被視為北美中部時間。若您有位在不同時區的日期/時間欄位，可以使用 Excel 公式將其轉換為北美中部時間 (美國/芝加哥)。

1. 新增您自己的名字、姓氏、實際電子郵件地址 (讓您可以收到在下一項任務中要傳送的培養電子郵件) 和工作職稱。將檔案儲存在您的電腦上。

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* 確保電子郵件地址僅包含 ASCII 字元。
   >
   >* Marketo **不**&#x200B;支援包含表情符號的電子郵件地址。
   >
   >* 透過 CSV 匯入 `NULL` 值，可能會在人員[活動記錄](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"}中的數值欄位產生「變更資料值」，_即使欄位已經為空白_。若您有任何[智慧行銷活動](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}使用「資料值已變更」篩選器或「資料值變更」觸發程序，則即使資料實際上並未變更，也可能會導致人員符合該行銷活動的資格。您可以使用[限制](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}來確保匯入時沒有人符合這些行銷活動的資格。

## 步驟 2：建立方案 {#step-create-a-program}

1. 前往「**[!UICONTROL Marketing Activities]**」區域。

   ![](assets/import-a-list-of-people-3.png)

1. 選取您的「**學習**」資料夾，然後在「**[!UICONTROL New]**」之下按一下「**[!UICONTROL New Program]**」。

   ![](assets/import-a-list-of-people-4.png)

1. 將方案&#x200B;**命名**&#x200B;為「我的商展方案」，並在「**[!UICONTROL Program Type]**」選取「事件」。

   ![](assets/import-a-list-of-people-5.png)

1. 在「**[!UICONTROL Channel]**」選取「**[!UICONTROL Tradeshow]**」，然後按一下「**[!UICONTROL Create]**」。

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>事件方案會在特定日期發生。了解更多關於&#x200B;[**事件**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}&#x200B;的資訊。

## 步驟 3：將您的試算表匯入 Marketo 中 {#step-import-your-spreadsheet-into-marketo}

1. 在「**我的商展方案**」中，按一下「**[!UICONTROL New]**」然後選取「**[!UICONTROL New Local Asset]**」。

   ![](assets/import-a-list-of-people-7.png)

1. 選取「**[!UICONTROL List]**」。

   ![](assets/import-a-list-of-people-8.png)

1. 將清單&#x200B;**命名**&#x200B;為「商展與會者」，然後按一下「**[!UICONTROL Create]**」。

   ![](assets/import-a-list-of-people-9.png)

1. 在您的「**[!UICONTROL Tradeshow Attendees]**」清單中，按一下「**[!UICONTROL List Actions]**」然後選取「**[!UICONTROL Import List]**」。

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >若您使用自己的 CSV 檔案，請確保其編碼為 UTF-8、UTF-16、Shift-JIS 或 EUC-JP。

   >[!NOTE]
   >
   >CSV 檔案的大小限制為 100MB。

1. 「**[!UICONTROL Browse]**」至您電腦上的 **tradeshow-attendees.csv** 試算表檔案，然後按一下「**[!UICONTROL Next]**」。

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >在清單匯入模式下，選擇「**[!UICONTROL Skip new people and updates]**」代表您不會影響現有的人員記錄，也不會記錄任何活動。若您想要一個快速、預先篩選的現有人員靜態清單供行銷活動使用，請使用此模式。選取此模式會：
   >
   > * 跳過建立新人員
   > * 跳過人員欄位更新
   > * 跳過活動記錄

1. 將您的「[!UICONTROL List Column]」欄位對應至其各自的 Marketo 欄位，然後按一下「**[!UICONTROL Next]**」。

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >為達到最佳的自動對應結果，欄標題應始終與欄位完全符合 (區分大小寫)。若您使用自訂欄位但在下拉式選單中沒有看到那些欄位，請返回並[建立欄位](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}，讓欄位能夠成為選項。

   >[!NOTE]
   >
   >若有任何您不想匯入的欄位，請在 Marketo 欄位下拉式選單中選取「**忽略**」。

1. 在「**[!UICONTROL Acquisition Program]**」選取「**我的商展方案**」，然後按一下「**[!UICONTROL Import]**」。

   ![](assets/import-a-list-of-people-13.png)

1. 等待您的人員匯入，然後關閉匯入進度快顯視窗。

   ![](assets/import-a-list-of-people-14.png)

1. 返回「**我的商展方案**」，按一下「**[!UICONTROL Members]**」索引標籤。您會看到剛才匯入的所有人員。

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>透過追蹤方案會籍，您可以分析方案的成功程度。了解更多關於&#x200B;[**方案**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}&#x200B;的資訊。

## 任務完成 {#mission-complete}

您的商展與會者現在是您 Marketo 方案的成員！

<br>

[◄ 任務 4：電子郵件自動回覆](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任務 6：點滴式培養 ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
