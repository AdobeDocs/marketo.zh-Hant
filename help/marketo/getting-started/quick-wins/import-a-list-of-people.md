---
unique-page-id: 2359418
description: 匯入人員清單 — Marketo檔案 — 產品檔案
title: 匯入人員清單
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 1b37a750c5e609b9e43e942df752305d85153989
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# 匯入人員清單 {#import-a-list-of-people}

## 任務：將貿易展會與會者的電子錶格清單導入資料庫 {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[設定並新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

在本教學課程中，您將學習如何將試算表檔案中的人員匯入Marketo。

## 步驟1:下載及編輯試算表 {#step-download-and-edit-a-spreadsheet}

1. 若要開始，請將我們慣用的試算表檔案([**tradeshow-theaders.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv))下載至您的電腦。

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >匯入日期時，請使用此格式：**9/21/20**（月/日/年）。

   >[!NOTE]
   >
   >匯入的任何日期/時間欄位都會視為中央時間。 如果您的日期/時間欄位位位於不同時區，則可使用Excel公式將其轉換為中央時間（美國/芝加哥）。

1. 新增您自己的名字、姓氏、電子郵件地址和職銜，然後將檔案儲存在您的電腦上。

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>在CSV檔案中輸入您的真實電子郵件地址，以便接收您將在下一個任務中傳送的培訓電子郵件。

## 步驟2:建立方案 {#step-create-a-program}

1. 前往&#x200B;**行銷活動**&#x200B;區域。

   ![](assets/ma-2.png)

1. 選擇&#x200B;**Learning**&#x200B;資料夾，然後在&#x200B;**New**&#x200B;下按一下&#x200B;**New Program**。

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **** 將方案命名為「我的貿易展會方案」，然後為「方案類型」選 **取「活動」**。

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. 為&#x200B;**Channel**&#x200B;選擇&#x200B;**Tradeshow**，然後按一下&#x200B;**Create**。

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>事件程式在特定日期發生。 深入了解&#x200B;[**Events**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md)。

## 步驟3:將試算表匯入Marketo {#step-import-your-spreadsheet-into-marketo}

1. 在&#x200B;**My Tradeshow Program**&#x200B;中，按一下&#x200B;**New**&#x200B;並選擇&#x200B;**New Local Asset**。

   ![](assets/seven-3.png)

1. 按一下&#x200B;**清單**。

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **** 將清單命名為「Tradeshow Atteders」，然後按一下「 **建立**」。

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. 在&#x200B;**Tradeshow Atteders**&#x200B;清單中，按一下&#x200B;**List Actions**&#x200B;並選擇&#x200B;**Import List**。

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >如果您使用自己的CSV檔案，請確定其編碼為UTF-8、UTF-16、Shift-JIS或EUC-JP。

   >[!NOTE]
   >
   >CSV檔案的大小限制為100MB。

1. **** 瀏覽至電 **腦上的tradeshow-tacteders.** csvspreadsheet檔案，然後按一 **下下一步**。

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >在「清單導入模式」中，選擇&#x200B;**跳過新人和更新**&#x200B;表示您將不會影響現有人員記錄或記錄任何活動。 如果您想要快速且預先篩選的現有人員靜態清單以用於行銷活動，請使用此模式。 選擇此模式將：
   >
   > * 略過建立新人員
   > * 跳過人員欄位更新
   > * 略過活動記錄


1. 將清單欄位對應至其各自的Marketo欄位，然後按一下&#x200B;**Next**。

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >欄標題應一律與欄位完全相符（區分大小寫），以取得最佳的自動對應結果。 如果您使用自訂欄位，但在下拉式清單中未看到這些欄位，請返回[建立它們](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)，使它們成為選項。

   >[!NOTE]
   >
   >如果有任何欄位不想匯入，請在「Marketo欄位」下拉式選單中選取「**忽略**」 。

1. 為&#x200B;**贏取方案**&#x200B;選取&#x200B;**我的貿易展會方案**，然後按一下&#x200B;**匯入**。

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. 等待您的人員導入，然後關閉導入進度彈出窗口。

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. 返回&#x200B;**My Tradeshow Program**，按一下&#x200B;**Members**&#x200B;標籤。 你會看見剛進來的人。

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>您可以追蹤方案會籍，以分析方案的成功。 深入了解&#x200B;[**程式**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)。

## 任務完成 {#mission-complete}

您的商展與會者現在是您Marketo計畫的成員！

<br> 

[◄任務4:電子郵件自動回應](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任務6:滴，滴，撫►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
