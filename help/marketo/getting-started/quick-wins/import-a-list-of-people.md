---
unique-page-id: 2359418
description: 匯入人員清單-Marketo檔案——產品檔案
title: 匯入人員清單
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 匯入人員清單{#import-a-list-of-people}

## 任務：將貿易展會與會者的試算表清單匯入您的資料庫{#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[設定並新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

在本教學課程中，您將學習如何將試算表檔案中的人員匯入Marketo。

## 步驟1:下載並編輯試算表{#step-download-and-edit-a-spreadsheet}

1. 若要開始，請將我們的練習試算表檔案([**tradeshow-tathenders.csv**](https://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv))下載至您的電腦。

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >匯入日期時，請使用下列格式：**9/21/20**（月／日/年）。

   >[!NOTE]
   >
   >匯入的任何日期／時間欄位都會視為「中央時間」。 如果您在不同時區有日期／時間欄位，則可使用Excel公式將其轉換為中時（美國／芝加哥）。

1. 新增您自己的名字、姓氏、電子郵件地址和職稱，然後將檔案儲存在電腦上。

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>在CSV檔案中輸入您的真實電子郵件地址，以便您收到在下次任務中傳送的有益電子郵件。

## 步驟2:建立程式{#step-create-a-program}

1. 前往&#x200B;**行銷活動**&#x200B;區域。

   ![](assets/ma-2.png)

1. 選擇&#x200B;**Learning**&#x200B;資料夾，然後在&#x200B;**New**&#x200B;下按一下&#x200B;**New Program**。

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **將** 方案命名為「我的商展方案」，並選取「活動」做為方 **案類型**。

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. 為&#x200B;**Channel**&#x200B;選擇&#x200B;**Tradeshow**，然後按一下&#x200B;**Create**。

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>事件程式在特定日期發生。 進一步瞭解&#x200B;[**Events**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md)。

## 步驟3:將試算表匯入Marketo{#step-import-your-spreadsheet-into-marketo}

1. 在&#x200B;**My Tradeshow Program**&#x200B;中，按一下&#x200B;**New**，然後選取&#x200B;**New Local Asset**。

   ![](assets/seven-3.png)

1. 按一下&#x200B;**List**。

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **將清** 單命名為「Tradeshow Atteders」，然後按一下「 **建立**」。

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. 在&#x200B;**Tradeshow Attedents**&#x200B;清單中，按一下&#x200B;**List Actions**&#x200B;並選取&#x200B;**Import List**。

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >如果您使用自己的CSV檔案，請確定它已編碼為UTF-8、UTF-16、Shift-JIS或EUC-JP。

   >[!NOTE]
   >
   >CSV檔案的大小限制為100MB。

1. **瀏** 覽至電 **腦上的tradeshow-tadenters.** csvspreadsheet檔案，然後按一下「下 **一步」**。

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >在清單匯入模式中，選擇&#x200B;**略過新人和更新**&#x200B;表示您不會影響現有人員記錄或記錄任何活動。 如果您想要快速、預先篩選的現有人員靜態清單以便用於行銷活動，請使用此模式。 選擇此模式將：
   >
   > * 略過建立新人
   > * 略過人員欄位更新
   > * 略過活動記錄


1. 將「清單列」欄位映射到各自的「Marketo欄位」，然後按一下「下一步」。****

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >欄標題應始終與欄位完全相符（區分大小寫），以取得最佳的自動對應結果。 如果您使用自訂欄位，但在下拉式清單中未看到這些欄位，請返回[建立](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)，以便成為選項。

   >[!NOTE]
   >
   >如果有任何您不想匯入的欄位，請在「Marketo欄位」下拉式選單中選取「忽略&#x200B;****」。

1. 為&#x200B;**贏取計畫**&#x200B;選擇&#x200B;**我的商展計畫**，然後按一下&#x200B;**匯入**。

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. 等待您的人員匯入，然後關閉匯入進度快顯視窗。

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. 回到&#x200B;**My Tradeshow Program**&#x200B;中，按一下&#x200B;**Members**&#x200B;標籤。 你會看到你剛引進的所有人。

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>您可以追蹤方案會籍，分析方案的成功。 進一步瞭解&#x200B;[**Programs**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)。

## 任務完成{#mission-complete}

您的商展參與者現在是您Marketo計畫的成員！

<br> 

[◄使命4:電子郵件自動回應](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[任務6:滴水，滴水，培養►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
