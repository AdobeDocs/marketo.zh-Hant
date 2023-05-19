---
unique-page-id: 2359418
description: 導入人員清單 — Marketo文檔 — 產品文檔
title: 導入人員清單
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 80512816eaf0a70a3f10a50c34aeea14edd9046b
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# 導入人員清單 {#import-a-list-of-people}

## 任務：將貿易展會與會者的電子錶格清單導入到資料庫中 {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[設定並添加人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

在本教程中，您將學習如何將電子錶格檔案中的人員導入Marketo。

## 步驟1:下載和編輯電子錶格 {#step-download-and-edit-a-spreadsheet}

1. 要開始，請下載我們的練習電子錶格檔案([**tradeshow-reqients.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"})。

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >導入日期時，請使用以下格式： **9/21/20** （月/日/年）。

   >[!NOTE]
   >
   >正在導入的任何日期/時間欄位都被視為「中心時間」。 如果日期/時間欄位位於不同的時區，則可以使用Excel公式將其轉換為中央時間（美國/芝加哥）。

1. 添加您自己的名字、姓氏、實際電子郵件地址（以便您能夠收到您將在下次任務中發送的培養電子郵件）和職銜。 將檔案保存在電腦上。

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >Marketo **不** 支援包含emoji的電子郵件地址。

## 步驟2:建立程式 {#step-create-a-program}

1. 轉到 **[!UICONTROL 營銷活動]** 的子菜單。

   ![](assets/import-a-list-of-people-3.png)

1. 選擇 **學習** 資料夾，然後在 **[!UICONTROL 新建]** 按一下 **[!UICONTROL 新程式]**。

   ![](assets/import-a-list-of-people-4.png)

1. **名稱** 「My Tradeshow Program（我的貿易展示計畫）」，並為 **[!UICONTROL 程式類型]**。

   ![](assets/import-a-list-of-people-5.png)

1. 選擇 **[!UICONTROL 貿易展]** 為 **[!UICONTROL 頻道]** 按一下 **[!UICONTROL 建立]**。

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>事件程式在特定日期發生。 瞭解有關 [**事件**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}。

## 第3步：將電子錶格導入Marketo {#step-import-your-spreadsheet-into-marketo}

1. 在 **我的貿易展計畫**&#x200B;按一下 **[!UICONTROL 新建]** 選擇 **[!UICONTROL 新建本地資產]**。

   ![](assets/import-a-list-of-people-7.png)

1. 選擇 **[!UICONTROL 清單]**。

   ![](assets/import-a-list-of-people-8.png)

1. **名稱** 清單「貿易展與會者」，然後按一下 **[!UICONTROL 建立]**。

   ![](assets/import-a-list-of-people-9.png)

1. 在 **[!UICONTROL 貿易展與會者]** 清單，按一下 **[!UICONTROL 列出操作]** 選擇 **[!UICONTROL 導入清單]**。

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >如果您使用自己的CSV檔案，請確保它已編碼為UTF-8、UTF-16、Shift-JIS或EUC-JP。

   >[!NOTE]
   >
   >CSV檔案的大小限制為100MB。

1. **[!UICONTROL 瀏覽]** 到 **tradeshow-reqients.csv** 在電腦上的電子錶格檔案，按一下 **[!UICONTROL 下一個]**。

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >在清單導入模式中，選擇 **[!UICONTROL 跳過新人和更新]** 意味著您不會影響現有人員記錄或記錄任何活動。 如果希望快速、預過濾的現有人員靜態清單用於市場營銷活動，請使用此模式。 選擇此模式將：
   >
   > * 跳過新人員建立
   > * 跳過人員欄位更新
   > * 跳過活動日誌記錄


1. 映射 [!UICONTROL 清單列] 欄位，然後按一下 **[!UICONTROL 下一個]**。

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >列標題應始終與欄位完全匹配（區分大小寫），以獲得最佳自動映射結果。 如果您使用自定義欄位，但在下拉清單中未看到這些欄位，請返回 [建立](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} 這樣它們就能成為選擇。

   >[!NOTE]
   >
   >如果有任何不想導入的欄位，請選擇 **忽略** 的子菜單。

1. 選擇 **我的貿易展計畫** 為 **[!UICONTROL 購置計畫]**，然後按一下 **[!UICONTROL 導入]**。

   ![](assets/import-a-list-of-people-13.png)

1. 等待您的人員導入，然後關閉導入進度彈出窗口。

   ![](assets/import-a-list-of-people-14.png)

1. 返回 **我的貿易展計畫**，按一下 **[!UICONTROL 成員]** 頁籤。 你會看到你剛引進的所有人。

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>您可以通過跟蹤程式成員資格來分析程式的成功。 瞭解有關 [**程式**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}。

## 任務完成 {#mission-complete}

您的貿易展與會者現在是您的Marketo計畫的成員！

<br> 

[◄任務4:電子郵件自動響應](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任務6:滴水，滴水，哺►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
